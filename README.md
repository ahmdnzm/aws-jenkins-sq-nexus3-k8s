# CICD with Jenkins SonarQube Nexus 3 Kubernetes

![architecture diagram](/images/architecture-diagram.png)

## Install Jenkins in AWS EC2

- Create Jenkins Server instance
    - Instance name called JenkinsServer
    - Instance type use t2.small
    - Create new keypair called jenkins-key
    - Create Security group called jenkins-SG
    - Inbound Securtiy Group Rules allow port 22 from My IP for ssh connection
    - Inbound Securtiy Group Rules allow port 8080 from My IP for Jenkins Web access
    - Other settings use default
- Launch instance
- Wait a few minutes to allow EC2 created

- SSH to JenkinsServer using jenkins-key
```shell
ssh -i jenkins-key.pem ubuntu@<jenkins public ip>
```






