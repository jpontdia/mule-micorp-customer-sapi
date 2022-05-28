# msdk-dynamicwhere
*Mule SDK - Dynamic Where Connector for data repositories like Salesforce or Relational Databases*
*<br><br>**This is an ongoing project!!**<br>*
## Table of contents
1. [Compilation Prerequisites](#compilation-prerequisites)
2. [Project Structure](#project-setup)
3. [Recommended content](#recommended-content)

## Compilation Prerequisites
To compile and build the project:
* Java Development Kit (JDK) 8. Must be version 8!
* Apache Maven, version 3.8 or later.
* IDE, Anypoint Studio or IntelliJ. To make changes to the code

Deployment in Anypoint Exchange:
* Anypoint account credentials


## Project Setup
The project was created using mule-extensions-archetype-maven-plugin version 1.3.1

Add next repository to your settings.xml
~~~xml
<repository>
   <snapshots />
   <id>mulesoft</id>
   <name>libs-release</name>
   <url>https://repository.mulesoft.org/nexus/content/repositories/public/</url>
</repository> 
~~~

In the parent directory where you want to create your project, open a terminal
window and run:
~~~bash
mvn org.mule.extensions:mule-extensions-archetype-maven-plugin:1.3.1:generate

[INFO] Scanning for projects...
[INFO]
[INFO] ------------------< org.apache.maven:standalone-pom >-------------------
[INFO] Building Maven Stub Project (No POM) 1
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] --- mule-extensions-archetype-maven-plugin:1.3.1:generate (default-cli) @ standalone-pom ---
* Enter the name of the extension (empty for default):
mulesdk-dynamicwhere-connector
* Enter the extension's groupId (empty for default):
com.jponte
* Enter the extension's artifactId (empty for default):
mulesdk-dynamicwhere-connector
* Enter the extension's version (empty for default):
1.0.0
* Enter the extension's main package (empty for default):

Using default value for property [package]
[INFO] Generating project in Batch mode
[INFO] Archetype repository not defined. Using the one from [org.mule.extensions:mule-extensions-archetype:1.2.0] found in catalog remote
....
....
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
~~~

To use the project in eclipse, run in the root folder of the project:
~~~bash
mvn eclipse:eclipse
~~~

## Usage
Add the dependency in the pom file of the new project
~~~xml
<dependency>
   <groupId>com.jponte</groupId>
   <artifactId>dynamicwhere-connector</artifactId>
   <version>1.0.0</version>
   <classifier>mule-plugin</classifier>
</dependency>
~~~

## Recommended content
* [Getting Started with the Mule SDK for Java](https://docs.mulesoft.com/mule-sdk/1.1/getting-started)

---
[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)