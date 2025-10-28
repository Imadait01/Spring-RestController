## Projet Gestion des Comptes Bancaires
## Description

Ce projet est une application RESTful développée avec Spring Boot pour gérer les comptes bancaires.
Il permet de créer, lire, mettre à jour et supprimer des comptes en utilisant JSON et XML comme format d’échange.



## Fonctionnalités

Créer un compte : POST /banque/comptes

Lire un compte : GET /banque/comptes/{id}

Mettre à jour un compte : PUT /banque/comptes/{id}

Supprimer un compte : DELETE /banque/comptes/{id}

Support pour JSON et XML

Validation des données

Retour d’un code HTTP approprié pour chaque opération (200 OK, 201 Created, 204 No Content, 404 Not Found…)


## Structure du projet
src/
├── main/
│   ├── java/ma/projet/banque/
│   │   ├── controller/
│   │   │   └── CompteController.java       
│   │   ├── entities/
│   │   │   └── Compte.java                 
│   │   ├── repository/
│   │   │   └── CompteRepository.java      
│   │   │   └── CompteService.java         
│   │   └── BanqueApplication.java         
│   └── resources/
│       ├── application.properties         
│       └── data.sql                        
└── test/
└── java/ma/projet/banque/
└── CompteControllerTest.java      



## Dépendances principales (pom.xml)
<dependencies>
<!-- Spring Boot Web pour REST -->
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-web</artifactId>
</dependency>

    <!-- Spring Data JPA pour persistance -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>

    <!-- H2 Database (en mémoire) -->
    <dependency>
        <groupId>com.h2database</groupId>
        <artifactId>h2</artifactId>
        <scope>runtime</scope>
    </dependency>

    <!-- Jackson XML pour supporter XML -->
    <dependency>
        <groupId>com.fasterxml.jackson.dataformat</groupId>
        <artifactId>jackson-dataformat-xml</artifactId>
    </dependency>

    <!-- Validation -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-validation</artifactId>
    </dependency>

    <!-- Tests -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-test</artifactId>
        <scope>test</scope>
    </dependency>
</dependencies>



## Lancer l’application

Cloner le projet

Ouvrir dans IntelliJ IDEA ou Eclipse

Lancer la classe BanqueApplication.java

L’API sera disponible sur : http://localhost:8082/banque/comptes