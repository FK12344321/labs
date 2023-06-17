# Docker 
### Description: 
Platform for containerization of the applications and services
### Purpose and benefits: 
Allows to automate the creation, delivery and management of the applications independant of operating system. This technology allows to isolate the application (to some extend) from the operating system, it lets to determine the describe the building process once, so it can be easily built by anyone who does not even know the stages of that build, also this is an essential part of k8s that builds uses the docker containers as a building block of the bigger systems. 
### Key features and functionalities 
Describe the building and launching process in one file, creation of an isolated container for an application, set the resources limit of the containers. 
### Use cases and examples
We can automate creation and launch of the services independent of the machine. For example, I build a visualization of the trading on my MacOS laptop for a customer who uses Windows. I can create a single docker compose file that combines all the services that get started automatically on the customer’s machine. 

We can control the services using the Docker desktop instead of the manual linux services configuration. For example, I can easily set the limits for the Elastic Search that obviously consumes too much resources 

We can use the docker containers in the k8s that knows how to build the new instances of our application (and control them) due to the Docker files. 
