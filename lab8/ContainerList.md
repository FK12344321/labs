## Docker commands 
To list docker containers I can use ```docker ps``` to display currently running containers (I do not have any right now)

<img width="507" alt="Screen Shot 2023-07-16 at 13 22 27" src="https://github.com/FK12344321/labs/assets/69464701/d416fa72-a8cb-4ec5-ab41-69f1ddb0b4d6">

Or ```docker ps -a``` to display all the containers currently present on my system 

<img width="1173" alt="Screen Shot 2023-07-16 at 13 23 40" src="https://github.com/FK12344321/labs/assets/69464701/ed745e1c-eb11-45cd-a2fe-c5cabf0282da">

I pulled the latest ubuntu image using ```docker pull ubuntu:latest``` command. After that I tried to remove the base image for that container with ```docker image rm ubuntu``` and got an error because the image was used by the container that I created

<img width="1165" alt="Screen Shot 2023-07-16 at 13 33 34" src="https://github.com/FK12344321/labs/assets/69464701/a0221f25-f242-4576-bdbb-1a3e628232af">
