# Spring Boot CMS with MongoDB

This project is a simple Content Management System (CMS) built using Spring Boot and MongoDB. It demonstrates the use of MongoDB's flexible document storage for hierarchical data structures, such as articles with nested comments and tags.

## Features

- Create, Read, Update, and Delete (CRUD) operations for articles
- Articles contain nested comments and tags
- Fast read and write operations using MongoDB
- Flexible schema design with MongoDB

## Technologies Used

- Spring Boot
- Spring Data MongoDB
- Lombok
- Maven
- MongoDB

## Requirements

- Java 8 or later
- Maven
- MongoDB

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/yourusername/spring-boot-cms.git
cd spring-boot-cms
```
### Configure MongoDB
Make sure MongoDB is running on localhost and port 27017. You can start MongoDB using the following command:
```bash
mongod --dbpath <your-db-path>
```
### Create the Database
Open the MongoDB shell and create the cms database:
```bash
mongo
> use cms
> db.createCollection('articles')
```
### Build and Run the Application
Use Maven to build and run the Spring Boot application:
```bash
mvn clean install
mvn spring-boot:run
```
### Project Structure
```bash
spring-boot-cms/
├── src/main/java/com/example/cms
│   ├── controller
│   │   └── ArticleController.java
│   ├── model
│   │   ├── Article.java
│   │   ├── Comment.java
│   │   └── Reply.java
│   ├── repository
│   │   └── ArticleRepository.java
│   ├── service
│   │   └── ArticleService.java
│   └── CmsApplication.java
├── src/main/resources
│   └── application.properties
├── .gitignore
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```
