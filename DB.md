Créer un docker-compose qui utilise l'image officiel de la db de votre choix:
### docker-compose.yml

```yaml
services:
  postgresql:
    image: bitnami/postgresql:latest
    ports:
      - "5432:5432"
    volumes:
      - postgres-data:/bitnami/postgresql
    env_file:
      - .env

volumes:
  postgres-data:
```

### .env
```bash
POSTGRESQL_PASSWORD=monmotdepasse
```

### Makefile

```bash
up: 
	docker compose up -d --build
down: 
	docker compose down
```


Etape a faire quand la DB est installer:
1. **Installer un ORM** (Sprint boot à dèja installer hibernate)
2. **Configurer la connexion** (URL dans `.env`)
3. **Créer le schéma** de BDD
4. **Utiliser l'ORM** dans tes Server Functions

2 Configurer la connextion (URL dans .env)
#### src/main/resources/application.properties
```
spring.datasource.url=jdbc:postgresql://localhost:5432/madb
spring.datasource.username=user
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
```
3 Crée le schéma de BDD

