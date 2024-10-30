# Zabbix 6.0 com Docker Compose
Neste projeto é disponibilizado arquivo docker-compose.yml, onde foi configurado containers contendo Zabbix-mysql, zabbix-server, zabbix-frontend, grafana e zabbix-agent. As imagens utilizadas são mysql:8.0, zabbix/zabbix-server-mysql:ubuntu-6.0.1, zabbix/zabbix-web-apache-mysql:ubuntu-6.0.1, grafana/grafana e zabbix/zabbix-agent2:alpine-6.0.1. 

Plugin do Zabbix já esta configurado para o container do Grafana.

Para subir os containers, execute o comando "docker-compose up -d"  na pasta onde está localizado o arquivo docker-compose.yml.

