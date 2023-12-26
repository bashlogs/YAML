# YAML
YAML Learning Repo

### Install requirements

```
pip install -r requirements.txt
```

### Run Python script
To Read **.yml** files
```
python read_yaml.py <filename.yml>
```

### Docker files
First build the docker image
```
docker build -t test5 .
```

### Docker-compose.yml
Docker compose is **a tool for defining and running multi-container Docker applications**.<br>
Run docker compose file
```
docker-compose up
```
Run docker compose file in background
```
docker-compose up -d
```
To check container is running or not
```
docker-compose ps
```
To stop the compose file
```
docker-compose down
```
### Dockerfile

All the manual steps happens in the docker-compose.yml file.

Docker run command

For application: 
```
docker run -e MONGO_URI=mongodb://mongodb2:27017/mydatabase --network network2 -p 3000:3000 -it app:dev
```

For mongodb: 
```
 docker run --name mongodb2 -p 27017:27017 --network network2 -v volume2:/data/db -e MONGO_URI=mongodb://mongodb2:27017/ mongo
```
