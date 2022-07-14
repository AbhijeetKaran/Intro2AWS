# What is AWS?
  - AWS (Amazon Web Services) is a comprehensive, evolving cloud computing platform provided by Amazon that includes a mixture of infrastructure as a service (IaaS), 
    platform as a service (PaaS) and packaged software as a service (SaaS) offerings. AWS services can offer organization tools such as compute power, database storage and content delivery services.
    
  Check out this Youtube video for a general introduction on AWS: https://www.youtube.com/watch?v=wWeyzYzd17o

## AWS terminologies
  - EC2 (Machines which computes)
  - S3 (Simple Storage Service)
  - AMI (Amazon Machine Image)
  - EBL (Elastic Load Balance)
  - ENI (Elastic Network Interface)
  - VPC (Virtual Private Cloud)
  - IGW (Internet gateway provided by Amazon)
  - IAM (Identity and Acess Management)
  - Subnets
  - Security groups
  - Route tables
  - key pairs
  - cloudwatch
  - IP address types for EC2 instances (EIP)

Follow this link to know about above terminologies: https://docs.paloaltonetworks.com/vm-series/9-1/vm-series-deployment/set-up-the-vm-series-firewall-on-aws/about-the-vm-series-firewall-on-aws/aws-terminology

## ECS
  Elastic Container Service (Helps to run docker images/instances on AWS cloud)
## EC2 
  Elastic Compute Cloud (Machine onto containers are spun[load and run])
## Fargate 
  It provides serverless option,helps run container on EC2 machines. Donot have to worry about the specifications of the Machine. ECS and fargate does that itself.
  
 Check out this Youtube video for better explanation on ECS, EC2 and Fargate: https://www.youtube.com/watch?v=DVrGXjjkpig

## Understanding containers
- Lets understand containers via dockers
  ### Docker
  Docker is a software platform that allows you to build, test, and deploy applications quickly. Docker packages software into
  standardized units called containers that have everything the software needs to run including libraries, system tools, code, and runtime
  (for example, dependencies). Using Docker, you can quickly deploy and scale applications into any environment and know your code will run.

## How docker works and why it's better than Virtual machines(VMs)?
Check out this Youtube video for understanding docker and VMs: https://www.youtube.com/watch?v=u-YWtdbpEhQ&t=3s

## Docker vs Conda
  From a high level both of them provide isolated fully-configurable environments allowing developers to avoid dependency resolution on any host computers.
  Docker’s concept of a registry is the very same as a package manager, except they deal in images and Dockerfiles rather than releases and source code.

  If you’re distributing software that can run in isolation, Docker may be for you.
  Docker runs software in isolation by distributing them among different containers, while conda runs all the needed software under one enviornment which is
  basically overlaid on top of ones system.
