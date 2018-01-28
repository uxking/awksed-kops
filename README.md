# awksed-kops
Repo for Docker image of kops to run Kuberentes cluster on AWS

Inlcudes kops and awscli

### Running the container
`docker run -id --name=awksed_kops --hostname=awksed-kops -v ~/kops:/root/kops awksed/kops`
