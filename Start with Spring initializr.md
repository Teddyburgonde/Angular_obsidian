Spring initializ te permet de créer l'architecture de son server (Tomcat).

Allez sur:
```bash 
https://start.spring.io/
``` 

```bash
Project -> Maven 
Language -> Java
Spring Boot -> 3.5.10
Group -> nomdedomaineictif.example
Artifcat -> Nom technique du projet ( Met le même que application)
Name -> Nom de ton application
Description -> Créer un back
Package name -> Jar
Configuration -> YAML
Java -> 21 (avant dans ton terminal verifie avec java --version si tu as bien la 21)
```

Dépendances à ajouter: 
```bash
1. Spring Web
2. Spring data JPA
3. PostgreSQL Driver

Appuyer sur generate !
```


application.yml 
Attention c'est que des espaces , pas de tabulation.
```yaml
spring:
  datasource:
    url: jdbc:postgresql://localhost:5432/db_back_2
    username: teddy
    password: 123
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
```

Créer la db:

```bash
psql -U postgres
CREATE DATABASE db_back_2;
\l -> verifie si la db existe
```



Lancer le server:
```bash
./mvnw spring-boot:run


aller sur :
http://localhost:8080/
```