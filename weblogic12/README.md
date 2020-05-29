
Antes da primeira execução vai ser necessario criar um base domain

docker run --name weblogic12 -it -p 7001:7001 -p 9002:9002 -e DOMAIN_NAME=base_domain  -v /mnt/d/work/docker/weblogic12:/u01/oracle/properties store/oracle/weblogic:12.2.1.4-dev 

