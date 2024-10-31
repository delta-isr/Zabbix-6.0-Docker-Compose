# Zabbix 6.0 com Docker Compose
Neste projeto é disponibilizado arquivo docker-compose.yml, onde foi configurado containers contendo Zabbix-mysql, zabbix-server, zabbix-frontend, grafana e zabbix-agent. As imagens utilizadas são mysql:8.0, zabbix/zabbix-server-mysql:ubuntu-6.0.1, zabbix/zabbix-web-apache-mysql:ubuntu-6.0.1, grafana/grafana e zabbix/zabbix-agent2:alpine-6.0.1. 

Plugin do Zabbix já esta configurado para o container do Grafana.

# Instalação
Para subir os containers, execute o comando "docker-compose -p Zabbix -f docker-compose-zabbix.yml up -d"  na pasta onde está localizado o arquivo docker-compose-zabbix.yml.

Explicando o comando:

-p: define um nome para o projeto (no caso no comando esta definido como Zabbix, mas você poderá colocar o nome que quiser)

-f: especifica o arquivo YAML a ser utilizado ao inves do padrão "docker-compose.yml"

up: inicializa os containers definidos no arquivo de composição.

-d: executa os containers em modo "detached", ou seja, em segundo plano. Não sera exibido no terminal atual os logs.



Caso queira personalizar a configuração basta editar o arquivo docker-compose-zabbix.yml usando VSCode.

