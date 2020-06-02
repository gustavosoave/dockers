
#To build this image use the follow command
docker build -t wildfly15:coprel-01 .

#To crate this container use the follow command
docker run --name wildfly15 -p 8080:8080 -p 9990:9990 -d wildfly15:beta  /opt/jboss/wildfly/bin/standalone.sh -b 0.0.0.0 -bmanagement 0.0.0.0  

#To check ports 
docker port wildfly15

#To start 
docker start wildfly15

#To stop
docker stop wildfly15

#To execute bash
docker exec -it wildfly15 bash



