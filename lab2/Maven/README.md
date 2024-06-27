# Maven 
### Description: 
Build automation tool for building Java projects 
### Purpose and benefits:
To simplify the building process of Java application by describing the rules for the build (for example code coverage limits), managing the dependencies . It is simple and maven repository contains a giant number of almost all the libraries that you could need 
### Key features and functionalities
A simple xml file to describe the building process. You can mention all the dependencies you need, so they get installed and resolved automatically, their version,  etc.  A large repository of the libraries that is very easy to work with. 
### Use cases and examples: 
We have a big application with dozens of dependancies. Insted of manually installing all of them manually as jar files and then resolving all the conflicts of their versions we can easily descibe everything in the pom.xml file 

We can make the maven to fail if the code coverage does not satisfy some standart, so we can use maven to ensure the code quality
