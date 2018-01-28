# awksed-kops
Repo for Docker image of kops to run Kuberentes cluster on AWS

Inlcudes kops and awscli

### Running the container
`docker run -id --name=awksed_kops --hostname=awksed-kops -v ~/kops:/root/kops awksed/kops`

### Logon to the container
`docker exec -it awksed_kops bash`

### Follow the documentation to build your first cluster
https://github.com/kubernetes/kops/blob/master/docs/aws.md#aws
