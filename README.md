# RunDeck

RunDeck in a container with WSO UEM APIs

Usage:
Building:

```Docker
docker build . -t rorymurdock/wso-uem-rundeck:latest
```

Running:

```Docker
docker run --name=rundeck -d -v ~/docker/data:/home/rundeck/server/data -v ~/docker/config:/home/rundeck/server/config/ -p 4440:4440 rorymurdock/wso-uem-rundeck:latest
```

If this is your first time running this container you will need to create a `config/realm.properties` so you can login. See the example file in this repo. It has the WSO UEM API modules + python3 already installed
