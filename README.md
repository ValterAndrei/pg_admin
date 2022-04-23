# Starting pgAdmin

1. Create the network
```
$ docker network create my-app
```

2. Insert the _network_ in your `docker-compose.yml` project
```
networks:
  default:
    external:
      name: my-app
```

3. Build and up the pgAdmin

```
$ docker-compose up pgadmin-compose
```

4. Access the pgAdmin in your browser

```
http://localhost:16543
```

5. Creating a server

```
Host name/address:    db
Port:                 5432
Maintenance database: app_development
Username:             postgres
```
