
Antes da primeira execução vai ser necessario criar um base domain

docker run --name weblogic12 -it -p 7001:7001 -p 9002:9002 -v /mnt/d/work/docker/weblogic12:/u01/oracle/properties store/oracle/weblogic:12.2.1.4-dev /bin/bash

Já dentro do domain será necessário definir o nome do dominio 

export DOMAIN_NAME=base_domain
./createAndStartEmptyDomain.sh
