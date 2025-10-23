# Komodo Setup

## requirements
* Ubuntu Server (basic install with SSH access)
* Docker (with compose plugin)
* GPU Drivers (if needed)

## getting started
1. Install ubuntu
2. Login to the new server and update
3. Install Docker
4. create a new folder for the compose files in the home directory
5. copy the compose.yaml and compose.env file from the mgmt_containers/komodo folder in the repo. 
6. Review the yaml and env files for any altercations that need to be made. 
7. From that directory run 'docker compose up -d' to pull and start the container. 
8. Once it is deployed, open a browser and navigate to hostip:9120 
9. Fill in the sign in boxes and click sign up. This will create the initial account. Sign ups will be disable after this account is created.

## post install 
1. Navigate to settings > providers and add account information that has access to the game-configs repo
2. Navigate to repos and add the game-configs repo
3. Navigate to syncs and add 2 syncs. One for the game_servers folder and one for the mgmt_severs folder. Once these are add execute the syncs to create all the needed stacks. 
