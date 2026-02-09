https://start.spring.io/

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



Dépendances à ajouter: 

1. Spring Web
2. Spring data JPA
3. PostgreSQL Driver

Appuyer sur generate !

Lancer le server:
./mvnw spring-boot:run