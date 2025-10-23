**NOTE**
* Files are configured in the game server repo. There is not much you need to configure elsewhere. Make changes and push the files to the repo.

## Terminology
* Komodo - Docker management interface
* Stack - What komodo calls docker compose
* Sync - Allows you to build toml files with stack configurations to deploy quickly

## Deploying Servers
* Login into komodo
* Browse to stacks and select one
* Click Deploy and enjoy!
  * If this is the first time launching the stack, komodo will say the stack deployed with errors. Ignore this for now. This is due to docker needing to create the volumes for the container. Part of the komodo deployment copies the LGSM and game config files after container creation. 
  * Once the server has fully installed the game. Redeploy it and there should not be an error. 

## Creating new stacks
* There are a couple files that need to be created at a minimum to deploy a stack. Below is where they need to be located:
  * Create a folder inside the game-configs directory with the LGSM name of the server (for example the name for a Counter Strike 2 server is cs2server). If there are spin offs of the main server (ie. a dedicated gun game server) name the folder cs2server-gungame.
    * Inside this folder with be a file named compose.yaml. Your compose script file must be named compose.yaml.
  * In the game-configs directory navigate to mgmt_containers/komodo. Inside this directory is 2 folders named game_servers and mgmt_servers. This is where a toml file with the same name as the server is created. This file is what setups up the stack to use the compose file we just created. Place toml files in thier respective folders. 
  * If there are containers we are no longer using, I move them to the notinuse folder inside the mgmt_containers directory. 
  * Once all relevant files have been created, push the changes to the repo. 
  * Open up komodo and browse to syncs. Select the sync folder you created the previous toml file in. This will pull that toml file and ask you to execute the sync to pull in the config.
  * Jump to "Deploying Server" part of this guide now.