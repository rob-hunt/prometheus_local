# run a prometheus / grafana stack locally, for metrics / visiblity / alerting development 

This project borrows heavily from the grafana turorials found at [grafana.com/tutorials](https://grafana.com/tutorials).

## Prequisites


Docker / docker compose installed locally :
- [Docker](https://docs.docker.com/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

If you're running Docker for Desktop for macOS or Windows, Docker Compose is already included in your installation.

## Running prometheus / grafana locally : 
```
docker-compose up -d
```

Grafana runs [here](http://localhost:4000) : http://localhost:4000
Promethesus runs [here](http://localhost:9090) : http://localhost:9090

Grafana default user : admin
Grafana default passowrd : admin
(the first time you log in you will be asked to change your password)

You must add a data source to grafana : 
- [click the gear icon](http://localhost:4000/datasources)
- [click add a data source](http://localhost:4000/datasources/new)
- click "prometheus"
- enter "http://prometheus:9090" for the URL
- click "Save & Test"
