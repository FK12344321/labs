### Size comparison 
To archive the ubuntu image I used command ```docker save ubuntu | gzip > ubuntu.tar.gz``` 

To get the unarchived image size I used ```docker image ls | grep ubuntu``` command and got the size of 69.2M 

<img width="656" alt="Screen Shot 2023-07-16 at 14 01 59" src="https://github.com/FK12344321/labs/assets/69464701/e78f2d13-6c9f-4d96-8db4-401bc27acd87">

Then I used ```ls -lh``` to find the size of the archived image that was 26M. 

<img width="520" alt="Screen Shot 2023-07-16 at 14 02 41" src="https://github.com/FK12344321/labs/assets/69464701/a0f1bd12-9420-44a7-9b5a-06e9caed2843">

Due to the archiving the image with gzip I reduced the image size by half 
### Nginx Container
I used command ```docker run --name nginx nginx``` to run the nginx container. The image was not found locally, so the docker fetched it from the docker hub. 

Afetr that I used ```docker run -p 80:80 --name nginx_container -d nginx``` to run the container on the port 80 in the detached mode. I opened the Chrome, followed the http://localhost:80 and made sure the nginx was running 

<img width="1164" alt="Screen Shot 2023-07-16 at 14 08 00" src="https://github.com/FK12344321/labs/assets/69464701/0263569d-84f7-4cbb-9ce3-1d39dd956dad">

Then I created the docker file with the index.html file with the crorresponding content from the task description and used the command ```docker cp index.html nginx_container:/usr/share/nginx/html/``` to copy it to the running container. 

<img width="932" alt="Screen Shot 2023-07-16 at 14 16 08" src="https://github.com/FK12344321/labs/assets/69464701/956791dd-c99a-4280-935e-d6fac044f2ef">

I created a new image with ```docker commit nginx_container```, got the id of it and taged it with ```docker tag d0903223be8677a75e61e10c64f521c6a82faf6a149346baecf8fc0985adf58c my_website```. I checked the images and greped my new image 

<img width="649" alt="Screen Shot 2023-07-16 at 14 21 28" src="https://github.com/FK12344321/labs/assets/69464701/0f603f47-c3a9-47b4-84ab-7b2b0a372997">

I stoped and removed the running container with ```docker stop nginx_container &&  docker rm nginx_container ``` and created a new one with ```docker run -p 80:80 --name nginx_container -d my_website```. I requested the html page and got the following result 

<img width="471" alt="Screen Shot 2023-07-16 at 14 24 50" src="https://github.com/FK12344321/labs/assets/69464701/563bf3e3-6283-477c-8558-707d629ff549">


After running ```docker diff nginx_container``` and here is the output 

<img width="491" alt="Screen Shot 2023-07-16 at 14 43 41" src="https://github.com/FK12344321/labs/assets/69464701/7ca9a05a-98f4-4600-a4c5-f1991bc52ae8">

If I ran the command for the initial docker container there would be more changes due to the index.html file, but this file is already injected in our new image, so the command did not show this. Howere default.conf file has been changed due to the options of the ```docker run``` command that overrided some of the default configurations
