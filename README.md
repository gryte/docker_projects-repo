# docker_projects-repo

Docker Project Repository

# common commands

*navigate to  where compose files are kept*
*ex.*
```bash
cd /app/config
sudo su -
```

|command|description|
|-------|-----------|
|`docker-compose --file sonarr.yml up -d`|bring up sonarr compose file in background|
|`docker-compose --file couch.yml up -d`|bring up couch compose file in background|
|`docker-compose --file unifi_ctrl.yml up -d`|bring up unifi controller compose file in background|
|`docker-compose --file jenkins.yml up -d`|bring up jenkins lts compose file in background|

# misc

## jenkins

need to ensure the volume on the host has the correct permissions for the jenkins user in the container

```bash
# set default jenkins container user:group on mapped volume
# this happens to exist as the alinkous user:group on the host
sudo chown 1000:1000 /app/config/jenkins
```
