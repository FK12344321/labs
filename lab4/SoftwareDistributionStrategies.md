## Definition of software distribution  
Software distribution is a mechanism of delivering our software and its updates to our users. It is important because it lets the developers get their projects working on the target devices of the users and help them to distribute their product. 

## Ways to distribute software 
1) Physical storage devices. Not flexible, do not allow to update the software and fix the bugs, hard to distribute, user has to have compatible readers, do not require internet connection 
2) Downloads from the website. Easy to download, easy to update by downloading a newer version, possible to read reviews on the web resource. 
3) Application stores. Controlled by the distributor, usually monopoly, takes big fees to distribute the project, easy to use, understandable interface 
4) Package managers.  Flexible (can be easily configured), requires some knowledge to use it, helps to automate the development process, useful while development, usually manages conflicts 
5) Source code. Requires certain skill set to build it, usually forces the user to troubleshoot, can be updated by the user, the code can be read by the user
6) Executable files. Very hard to decompile the code to read it, easier to launch, as it does not need the user to build the project, but still not so user friendly 
7) Container. Usually does not depend on the machine of the user, requires some system to control containers like Docker, easy to orchestrate, can be used for automation of the deployment if you need more than one node, useful for developers and DevOps engineers 

## Best practices 
1) use VCS to manage the versions of the project 
2) release management to determine a proper way to manage the steps of the release 
3) collect analytics and user feedback to control the quality of the product 
4) make the releases secure by implementing the security automated checks and limiting the rights of the people who have access to the project 
5) automate deployment by CI/CD tools to increase the code quality and delivery speed 
6) make documentation to make the project more accessible and easy to use 
