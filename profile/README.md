# Venade Hytale

<img width="1253" height="392" alt="image" src="https://github.com/user-attachments/assets/fb1ef19d-038f-4efe-987e-26368ad8547b" />

<img width="760" height="791" alt="image" src="https://github.com/user-attachments/assets/8b3fd1e5-2c43-42a5-8425-8399b2b4dde1" />



## Services
### Player-Service 
Player: 
- id
- name
- role (admin/dev/vip/normal)
- coins?
- created_at
- last_join_at
- last_country?
- language?
- current_server_id

### Statistics-Service
Stats:
- statistics<string, obj> 

Funktionen:
- CRUD
- Top10
- Rank (#1/1000)

### Cloud Service
GameGroup:
- PK Name 
- slots
- min server
 
GameServer:
- uuid
- id 1
- name Lobby
- ip/node
- port
- slots
- current_player_count
- State(STARTING, READY, IN_GAME, FULL, STOPPING, UNKNOWN)
- FK groupName
- List of Players?

Functions:
- getGameServerById(id)
- getAllGameServers()
- getAllGameServersByGroup(group)
- getServerWithLowestUsageByGroup(group)
- getState(id)
- getOnlineCound(group)
- getOnlineCound(id)
- getOnlineCoundPercentage(id)


Interacts with Kubernetes API (e.g. for managing replica count)


## Questions
- Healthcheck: Via Kubernetes AND gRPC
- How does a gameserver know which server he is? environment
- How does a gameserver know on which port to start? all start on default - venade API 
- Join - which Server?

## Roadmap
- Player Service
- Cloud Service
- VenadeAPI (gRPC Client testen)
- Redis einbauen

---
