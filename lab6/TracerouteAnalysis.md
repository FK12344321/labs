## Traceroute Analysis
To trace route to my.university.innopolis.ru I used ```traceroute``` command (on mac)
<img width="625" alt="Screen Shot 2023-07-09 at 17 53 56" src="https://github.com/FK12344321/labs/assets/69464701/76a0db60-edf2-47cb-8d26-4ab185eaabb3">

The entries in the list are hops that the packet go through on the way to the destination host. Looks like the request did not go outside of the university network, as all the ip addresses were private

## DNS lookup 

I used ```nslookup``` command to perform a DNS lookup of the same host. 

<img width="504" alt="Screen Shot 2023-07-09 at 18 04 52" src="https://github.com/FK12344321/labs/assets/69464701/eafbfd97-0585-4259-82ec-51421bd5de92">

The command performed the lookup and found the ip address of the hostname and it is 192.168.1.254 
