### Starting pgAdmin

1. Build and up the pgAdmin

```bash
docker compose up pgadmin-compose
```

2. Access the pgAdmin in your browser

  - http://localhost:16543


3. Creating a server

```
Host name/address:    db
Port:                 5432
Maintenance database: app_development
Username:             postgres
```

---

### Hint

Find the current network of your project's database and replace the network in the [`docker-compose.yml`](/docker-compose.yml) file.

```bash
docker ps --format '{{ .ID }} {{ .Names }} {{ json .Networks }}'
```
