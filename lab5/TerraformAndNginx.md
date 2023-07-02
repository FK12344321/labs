## Version 
Terraform v1.5.2
## Steps to install 
I used manual installation following the instructions here: https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli . I downloaded 
a zip with an executable file inside. I executed it and moved it to the /usr/local/bin/  with ```mv ~/Downloads/terraform /usr/local/bin/```. After that it was installed and I could use the command ```terraform```

P.S. I had to use VPN to download the zip 
## Commands 
```terraform --version``` to check the version 

```terraform init``` to initialize the working directory 

```terraform apply``` to apply the config files 

## Challenges 
I had to use VPN to use the terraform. 

Nginx latest version did not work, so I had to use v1.21.0 
