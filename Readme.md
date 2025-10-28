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
     
<img width="437" height="607" alt="Screenshot 2025-10-28 024015" src="https://github.com/user-attachments/assets/ae14bbaf-f948-427b-97fa-f0f175dc9d36" />



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



<img width="1919" height="669" alt="TP8" src="https://github.com/user-attachments/assets/368dba41-8e3e-460a-aa53-f09f94f87891" />

<img width="1900" height="1008" alt="TP8 1" src="https://github.com/user-attachments/assets/88f8c0eb-efac-472d-984b-59bd5f564448" />

<img width="1900" height="953" alt="TP8 2" src="https://github.com/user-attachments/assets/bee2bd65-1062-4082-ba88-f09fa3b001a8" />

<img width="1403" height="957" alt="TP8 3" src="https://github.com/user-attachments/assets/d403943f-9bc4-4d01-b6f5-9fbc90388ed7" />

<img width="1441" height="648" alt="TP8 5" src="https://github.com/user-attachments/assets/19e610ae-f540-45a3-a049-ee4d6d2638da" />

<img width="1463" height="711" alt="TP8 6" src="https://github.com/user-attachments/assets/b1c232e7-bf3e-4f6b-90df-1b0382c0f4a0" />

<img width="1463" height="849" alt="TP8 7" src="https://github.com/user-attachments/assets/16abdf0d-3016-4fd9-a2d1-0ea90c82f8d7" />

<img width="1455" height="740" alt="TP8 8" src="https://github.com/user-attachments/assets/331b4da3-c854-44c7-9583-7e38da4cd09a" />

<img width="1463" height="639" alt="TP8 9" src="https://github.com/user-attachments/assets/31ed5aa5-1a8b-4261-91d5-2f049451b3c3" />

<img width="916" height="480" alt="TP8 10" src="https://github.com/user-attachments/assets/f00c95ef-f9de-40a4-8324-be7300f5a881" />









