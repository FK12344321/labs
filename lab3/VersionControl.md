## Definition
Version control system is a service that allows a team or a single developer to manage the changes and versions of their / his project: to save the previous versions, to create several versions of the same project, to merge them etc. Its purpose is to simplify the development process, make the team work on the project easier, to keep the project stable and mainly control the versions and its history. 
## Benefits and advantages of using version control in a collaborative environment
1) Using the VCS significantly simplifies the team work on the same project, as each member of a team is able to work on the and develop his features in a separate version (branch)
2) You can checkout all the changes and get back to the stable version if something goes wrong
3) The team can keep a separate stable branch
4) The VCS usually provides developers with very useful tools for comparing their versions and merging them
5) Pull requests mechanism facilitates the code review and improves the code quality 
6) Protected branches and rights mechanism also improves the code quality and make the development safer and more secure
## VCS types 
#### Local VCS  
All the versions are stored locally on one machine and represented by the project itself and the changes made to it. This type of VCS is unsafe, as everything can be lost if the local machine gets destroyed. It also very inconvenient for the team work, as the local VCS makes it difficult to collaborate  
#### Centralized VCS
In the case of Centralized VCS everything is stored on one centralized server, so the team members can access the changes and commit directly to that server. The versions are stored on that server, so if it gets destroyed, all the progress gets lost if the developers did not happen to save anything locally. Compared to the Local VCS, centralized one makes the team work easier because all of the members have access to the server. 
#### Distributed VCS
While working with distributed VCS all the team members have a mirrored version of the project locally and their version can differ from the other members’ version. At the same time the project is stored on the server, so new team members can clone it and pull from it. It makes the team work easier. Team members can work on the project locally and then merge them with each other’s versions 
## VCS comparison
#### CVS 
One of the oldest VCS was released in the 80s. This VCS is quite mature and does not require many updates as it has been developed for a very long time and became very mature. Branch mechanism is not suitable for short term branches that makes the team work harder
#### Apache Subversion 
Was developed on the basis of the CVS and improved many of its disadvantages. Introduced the concept of atomic operation that led to the reduction of the code inconsistency (while applying changes all of the changes are applied or none of them). Became a modern version of CVS. More instruments work with it compared to CVS 
#### Git 
Became de facto leader of the market. Made a revolution in the world of VCS. There is a lot of information on the internet on how to work with it, many plugins and a very user-friendly interface. It is decentralized, so it is easier to work with the projects locally. Significantly increased the speed of branch operation compared to Subversion and CVS. 
#### Mercurial 
Also distributed, so it keeps all the advantages of this type of VCS. Not so well developed as Git (so not so many features are implemented). Better documentation than Git and easier to learn rather than Git. 
