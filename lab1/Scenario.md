## Scenario 
A team developing a young but rapidely growing social media with a development team and one admin that does not use any DevOps practices 

## Challenges and solutions 
### Challenge 1: 
With the growth of the product gets competitors and the team realizes that the product requires frequent releases with bug fixes and new features.  Unfortunately, the admin who deploys all these is not always available, so the team has to wait. Additionally, the developers who are responsible for testing the code before the deployment often forget about it and ignore the linters’ hints while development worsens the overall code quality and increases the technical debt. 
### Solution: 
They could create a CI/CD pipeline (for example, GitLab CI) that ensures the code quality before the deployment and does the deployment that would increase the code lower the tech debt and increase the speed of the updates delivery. 
### Challenge 2: 
Sometimes the incidents occur (for example, the number of 5xx responses gets too big), but  the team does not notice them immediately. They find out about the incidents only from secondary sources such as users’ feedback. 
### Solution: 
We can start a Prometheus server that pulls the metrics from our services and imports them to Grafana. Grafana will visualize them, so the observability of the system gets increased. The admin or the developers can immediately see the unusual behavior of the system, so they can for example, roll back to the previous more stable release and avoid the degradation of the user experience. 
### Challenge 3:
Every time the team encounters some incidents, they find a person and blame him for this. The person gets demotivated and finally, nobody wants to take the responsibility and tries to shift the blame to the other members of the team. As a result, the atmosphere in the office gets toxic, people are unmotivated and they actually do not solve the reasons for the incidents. 
### Solution: 
They can introduce blameless culture and try to analyze the reasons for the problems. For example, instead of blaming the developer for the bugs caused by the pure testing, they can introduce the test coverage check as a part of the pipeline and really solve the problem 

<b> P.S. some of the solutions combine several practices from the DevOps_Practices.md </b>
