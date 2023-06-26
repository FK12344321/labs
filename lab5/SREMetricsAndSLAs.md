## SRE metrics 
<b>SLA</b> is a service level agreement on the metrics that the provider guarantees and the penalties in case of violation 

<b>SLO</b> is a service level objective. In other words this is a performance that we seek to achieve 

<b>SLI</b> is a service level indicator. Basically these are the metrics that we use to evaluate SLO 

## SLA of Google and GitHub
Here is the <a href=https://cloud.google.com/translate/automl/sla>link</a> to the google auto ML translation service. It guarantees 99.9% uptime percentage. It means that the company guarantees that the service can be down only 0.01% of all time. It also states that in case of violation clients can get financial credits, such as 10% discount in case of the uptime being 99.0 - 99.9 or 25% discount if the uptime is only 95 - 99%  

GitHub <a href=https://github.com/customer-terms/github-online-services-sla>link</a> also gurantees 99.9 percent uptime of the basic functions such as pull requests, github issues, webhooks, pages and etc. It gives 10% return if the uptime is between 99 and 99.9 and 25% if it is less then 99%. It is also calculated by the time unavailable devided by the available time. 

In case of GitHub actions the values for the uptime is the same, but it is calculated differently. It is the ratio of successful triggered executions to the total number of executions. 

Discovered facts: I found out that different services use different metrics to evaluate the qulity of the user experience. 
