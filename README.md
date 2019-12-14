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
|`docker-compose --file jackett.yml up -d jackett`|bring up jackett compose file in background|
|`docker-compose -f <file.yml> up -d --no-deps --build`|update image and restart container in one command|

# update and restart container

```bash
docker-compose up -d --no-deps --build <service_name>
```

