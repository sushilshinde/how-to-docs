
1. Install docker on your OS https://docs.docker.com/engine/install/

2. Execute this instruction on command line
```
docker run -it --name ifx --privileged -p 127.0.0.1:9088:9088 -p 127.0.0.1:9089:9089 -p 27017:27017 -p 127.0.0.1:27018:27018 \
-p 127.0.0.1:27883:27883 -e LICENSE=accept -e DB_INIT=1 ibmcom/informix-developer-database:latest
```
3. Execute this instruction on command line `docker exec -it <CONTAINER ID> bash`

4. run `dbaccess` to create your databases

5. Connect from DBvisualizer 

![alt text](https://raw.githubusercontent.com/sushilshinde/how-to-docs/main/assets/db-viz-docker-ifx.png)

6. Here are the password details : https://github.com/informix/informix-dockerhub-readme/blob/master/12.10.FC12/informix-developer-database.md 

