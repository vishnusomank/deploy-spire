# SPIRE deployment files

This repository contains the kubernetes deployment files for spire server and agent.


## Images used

|Sl. No.|Image Name | Purpose | Image |
|--|--|--| -- |
| 1. | ***Spire Agent*** | To initialise spire agent. | [knoxuser/spire:agent](https://hub.docker.com/repository/docker/knoxuser/spire/general)  |
| 2. | ***Spire Server*** | To initialise spire server. Uses version 1.5.1 |[knoxuser/spire:server](https://hub.docker.com/repository/docker/knoxuser/spire/general)  |
| 3. | ***Spire Server Sidecar*** | To add default entries to spire server and to generate the initial spire agent join_token. Also regenerates join_token if spire agent is down for more than a predefined time. |[knoxuser/spire:sidecar](https://hub.docker.com/repository/docker/knoxuser/spire/general)  |
| 4. | ***Wait For It*** | To stop initialising spire agent until spire server is up and running |[knoxuser/spire:wait-for-it](https://hub.docker.com/repository/docker/knoxuser/spire/general)  |