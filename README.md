# Spring Boot Application for Maven Practice

## Introduction

This repository contains a **Spring Boot** application configured with a pre-built **Maven** `pom.xml` file. It's designed for practicing Maven tasks like building, testing, managing dependencies, and packaging Spring Boot applications.

The goal is to help you practice key Maven tasks using a fully functional Spring Boot project.

## Prerequisites

Make sure you have the following installed on your machine:
- **Java 8 or higher**
- **Maven 3.6+**: [Download Maven](https://maven.apache.org/download.cgi)

# Steps to install Maven on Linux

``` shell
Step 1: Update local packages

sudo apt update && sudo apt upgrade -y 

Step 2: Install JDK

sudo apt install  openjdk-11-jdk or sudo apt install fontconfig openjdk-17-jre

Step 3: Verify Installation

java --version

Step 4: Install Maven.

sudo apt install maven -y

Step 5: Verify Installation

mvn --version


```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/JM-TEFFU/springboot-application.git
cd springboot-application

```
##  Explore the pom.xml File
vim pom.xml 

# Steps to build artifacts or jar file

## 1. Run Maven Clean
The first step before building the project is to clean any previously compiled files and resources. This ensures that the build is fresh

`$ mvn clean`

This command removes the target/ directory where compiled files are stored.

## 2. Compile the Project
Next, compile the source code into .class files. Maven will also download any missing dependencies specified in the pom.xml:

`$ mvn compile`

This command compiles all the Java source files in the src/main/java directory.

## 3. Run Unit Tests (Optional)
If you have unit tests in your project, you can run them before packaging:

`$ mvn test`

This ensures that your application is functioning correctly before you create the .jar file.

## 4.  Package the Project into a JAR
The most crucial step is packaging the compiled code and resources into a .jar file. Maven will package your Spring Boot application along with all its dependencies.

`$ mvn package`

- The default output of this step will be located in the target/ directory.
- The .jar file is created with a name format like springboot-maven.jar.


## 5. Verify the JAR File
Once Maven completes packaging, you can verify that the .jar file has been created:

`$ ls target/ `

You should see the .jar file listed among other build-related files.

## 6.  Run the JAR File
Now that the .jar file has been created, you can run the Spring Boot application using the following command:

`$ java -jar target/srpingboot-application.jar`

This command starts the Spring Boot application and opens it to the default port (usually 8080).

## Congragulations you have created your first artifacts using Apache Maven














