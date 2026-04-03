This Repo is for QA Test Management backed application using Java+Spring boot, JPA, PostgresSQL as database, Docker, Kubernetes, etc

Phase-1(Project Setup & PostgreSQL install)
-------------------------------------------

1.Download the Pre-Configured Maven based Springboot application with Java 17 as the Java version from Sprin Initlizer
2.UnZip the dowload and open the project in Intellij
3.Perform the mvn lifecyle with command as # mvn clean install.
4.Create the Following packages under /src/main/java
  a.controller               --> Entry point for the HTTP requests
  b.service and service.impl --> The Business logic layer with its implementation
  c.DAO and DAO.impl         --> Data Access object layer for pre/post business logic before/after the JPA repository and its implementation
  d.repository               -->  JPA Repository(Spring data)
  e.entity                   --> Create the Java object for the tables
  f.DTO, DTO.requests & DTO.responses --> Data transfer object for requests and responses
  g.exceptions               --> For Custom exceptions
  h.config                   --> security and bean configs
  i.util                     --> helper classes
5.Download and install the PostgreSQL and pgadmin
6.Open pgadmin and create a database #qatestmg
7.Create a application.yml under /src/main/resources and update the details like db url, username, password, jpa details like hibernate, ddl-auto etc, server port

