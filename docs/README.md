# LAN All Night Docker 

* [Komodo Setup](guides/komodo_setup.md)
* [Deplyment/Creation](guides/docker_deployment.md)
* [Network Setup](guides/network_setup.md)

### SERVERS
| IP | DESC |
|----|------|
|.52| DOCKER - Management|
|.53| DOCKER - Media|
|.54| DOCKER - Game Server 1|
|.55| DOCKER - Game Server 2|

### SERVICES
| name | link | resolves |
|----|----|------|
| [Pangolin](./apps/pangolin.md) | https://pangolin.at.lanallnight.com | 192.168.50.52 |
| [Lanager](./apps/lanager.md) | https://intranet.at.lanallnight.com | pangolin |
| [Homepage](./apps/homepage.md) | https://servers.at.lanallnight.com | pangolin |
| [Restreamer](./apps/restreamer.md) | https://restreamer.at.lanallnight.com | pangolin |
| [Fireshare](./apps/fireshare.md) | https://clips.at.lanallnight.com | pangolin |
| [Komodo](./apps/komodo.md) | https://komodo.at.lanallnight.com | pangolin |
| [Technitium](./apps/technitium.md) | http://dns.at.lanallnight.com | 192.168.50.20 |
| Lancache | http://lancache.at.lanallnight.com | 192.168.50.2 |
| Check-In | https://checkin.at.lanallnight.com | 192.168.50.19 |

### Game Servers
| IP | SERVER |
| ------ | ----- |
| 50.56 | [Quake Live](games/qlserver.md) |
| 50.57 | [RTCW](games/rtcwserver.md)|
| 50.58 | [ETL](games/etlserver.md) |
| 50.59 | [Counter Strike 2](games/cs2server.md) |
| 50.60 | [Counter Strike 1.6](games/csserver.md) |
| 50.61 | [Rust](games/rustserver.md) |
| 50.62 | [Day of Defeat Source](games/dodsserver.md) |
| 50.63 | [Garry's Mod](games/gmodserver.md) |
| 50.64 | [Half Life 2 Deathmatch](games/hl2dmserver.md) |
| 50.65 | [Left 4 Dead 2](games/l4d2server.md) |
| 50.66 | [Team Fortress 2](games/tf2server.md) |
| 50.67 | [Minecraft Java](games/mcserver.md) |
| 50.68 | [Minecraft Bedrock](games/mcbserver.md) |
| 50.XX | [Unreal Tournament](games/utserver.md) |
| 50.69 | [Unreal Tournament 99](games/ut99server.md) |
| 50.70 | [Unreal Tournament 3](games/ut3server.md) |
| 50.71 | [Unreal Tournament 2004](games/ut2k4server.md) |
| 50.72 | [Battlefield 1942](games/bf1942server.md) |
| 50.73 | [Call of Duty 4 MW](games/cod4server.md) |
| 50.XX | [Palworld](games/pwserver.md) |
| 50.XX | [Project Zomboid](games/pzserver.md) |
| 50.XX | [Mordhau](games/mhserver.md) |
| 50.XX | [Satisfactory](games/sfserver.md) |
| 50.XX | [Arma 3](games/arma3server.md) |
| 50.74 | [Arma Reforger](games/armarserver.md) |