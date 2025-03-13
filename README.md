#### Follow [@YongkangHe](https://linktr.ee/k8sug)

I just want to build an EKS Cluster to play with the various Security and Data Management capabilities e.g. Security Scans, Backup/Restore, Disaster Recovery and Application Mobility. 

It is challenging to create an EKS cluster from AWS Cloud if you are not familiar to it. After the EKS Cluster is up running, we still need to install a sample DB, create policies etc.. The whole process is not that simple.

This script based automation allows you to build a ready-to-use EKS demo environment with PostgreSQL deployed in about 20 minutes with eks-deploy.sh. For simplicity and cost optimization, the EKS cluster will have only one worker node and create a separate vpc and subnets. This is bash shell based scripts which might only work on Cloud Shell. Linux and MacOS terminal may work as well, but I haven't tested it yet. 


# Here're the prerequisities. 
1. Go to open AWS Cloud Shell
2. Clone the github repo, run below command
````
git clone https://github.com/yongkanghe/eks-casa.git
````
3. Install the required tools (eksctl, kubectl, helm)
````
cd eks-casa;./awsprep.sh;. ./setenv.sh
````
4. Optionally, you can customize the clustername, instance-type, zone, region
````
vi setenv.sh
````

# EKS Cluster Automation 

1. To deploy an EKS cluster
````
./eks-deploy.sh
````

2. To destroy the EKS cluster after testing
````
./eks-destroy.sh
````

# Velero for EKS Automation 

1. 1 min to enable EKS Backup via Velero
````
./velero-deploy.sh
````

2. To clean up Velero for EKS
````
./velero-destroy.sh
````

# Secure EKS Containers via Falco 

````
./falco-deploy.sh
````

# Build an EKS cluster via Web UI
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/d0vhf_ggnko/0.jpg)](https://www.youtube.com/watch?v=d0vhf_ggnko)
#### Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

# Secure EKS Cluster & AWS Cloud
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Nvxbg4iGbJE/0.jpg)](https://www.youtube.com/watch?v=Nvxbg4iGbJE)
#### Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

# Secure your containers via Falco
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/v0NtUVUkfmQ/0.jpg)](https://www.youtube.com/watch?v=v0NtUVUkfmQ)
#### Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

# Build, Protect and Migrate Containers
[![IMAGE ALT TEXT HERE](https://pbs.twimg.com/media/FK5rsaeXwAIEmtI?format=jpg&name=small)](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ)
#### Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

# CloudCasa - Best Kubernetes BaaS
https://cloudcasa.io 

# Contributors

#### Follow [@YongkangHe](https://linktr.ee/k8sug) on LinkedIn, Twitter, WhatsApp, etc.
#### K8SUG meetup 26,000 members | Kubernetes Discussions 19,000 members
#### Yongkang LinkedIn 45,000 followers | kubestrong LinkedIn 28,000 followers
#### awstronaut LinkedIn 9,700 followers | K8SUG LinkedIn 14,000 followers


