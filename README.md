# awksed-kops
Repo for Docker image of kops to run Kuberentes cluster on AWS

Inlcudes kops, kubectl and awscli

### Running the container
Create a directory called "kops" (or whatever you want) somewhere on you local machine
For this example, there is a "kops" directory on the local machine's $HOME dir at ~/kops

`docker run -id --name=awksed_kops --hostname=awksed-kops -v ~/kops:/root/kops awksed/awksed-kops`

### Logon to the container
```
docker exec -it awksed_kops bash
cd /root/kops 
```
Create your [deployment|service|*].yaml files in /root/kops. If you remove the container at a later time, anything you placed in /root/kops will persist on your local machine's "kops" directory since we ran the docker container with the `-v` flag.


### Follow the documentation to build your first cluster
https://github.com/kubernetes/kops/
