![aws](https://user-images.githubusercontent.com/53552871/179160547-0ae063b2-cfb7-463a-8404-083644edd497.jpg)
# What is AWS?
  AWS (Amazon Web Services) is a comprehensive, evolving cloud computing platform provided by Amazon that includes a mixture of infrastructure as a service (IaaS), 
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

## EC2 
  Elastic Compute Cloud (Machine onto which containers are spun[load and run])
  AWS allows users to rent virtual computers(EC2) on which to run their own computer applications.
  
  EC2 encourages scalable deployment of applications through which a user can boot an Amazon Machine Image (AMI) to configure a virtual machine, which       Amazon calls an "instance".
  
  Instance comprises varying combinations of CPU, memory, storage, and networking capacity and give you the flexibility to choose the appropriate mix   of   resources for your applications.
  
  A user can create, launch, and terminate server-instances as needed, paying by the second for active servers – hence the term "elastic".
  
  ### Types of instances based on payment:
      - On-Demand Instances – Pay, by the second, for the instances that you launch.
      - Dedicated Instances – Pay, by the hour, for instances that run on single-tenant hardware.
      - Reserved Instances – Reduce your Amazon EC2 costs by making a commitment to a consistent instance configuration, including instance type and Region,       for a term of 1 or 3 years.
      - Dedicated Hosts – Pay for a physical host that is fully dedicated to running your instances, and bring your existing per-socket, per-core, or per-VM       software licenses to reduce costs.
      - Spot Instances – Request unused EC2 instances, which can reduce your Amazon EC2 costs significantly.
      - Capacity Reservations – Reserve capacity for your EC2 instances in a specific Availability Zone for any duration.
      - Savings Plans – Reduce your Amazon EC2 costs by making a commitment to a consistent amount of usage, in USD per hour, for a term of 1 or 3 years.
  
  Follow this link to know more about the pricing schemes of instances: https://aws.amazon.com/ec2/pricing
  
  ### Types of instances based on machine specifications (as of july 15 2022):
      - Mac
      - T4g
      - T3
      - T3a
      - T2
      - M6g
      - M6I
      - M5
      - M5a
      - M5n
      - M5zn
      - M4
      - A1
   Follow this link to know details about their specifications: https://aws.amazon.com/ec2/instance-types
  
## ECS
  Elastic Container Service is responsible for managing the lifecycle and placement of tasks.A task is usually made of one or two containers that work       together. One can ask ECS to start or stop a task, and it stores your intent. However, ECS does not run or execute your container. ECS only provides the   control plane to manage tasks. To run containers, you have two options. You can use ECS container instances, or you can use Fargate. Both options work     together with ECS.

## Fargate 
  It provides serverless option. It helps run container on EC2 machines. User do not have to worry about selecting the specifications of the Machine. ECS and fargate does that itself.
 
![Screenshot from 2022-07-15 12-34-44(1)(1)](https://user-images.githubusercontent.com/53552871/179169593-bb9fbf16-0048-4948-9546-ef31ce9e4499.png)

 Follow this link to know about ECS and Fargate, and their differences: https://cloudonaut.io/ecs-vs-fargate-whats-the-difference 
 Check out this Youtube video for better explanation on ECS, EC2 and Fargate: https://www.youtube.com/watch?v=DVrGXjjkpig

## Understanding containers
   Let's try understanding containers via dockers
  ### Docker
  Docker is a software platform that allows you to build, test, and deploy applications quickly. Docker packages software into
  standardized units called containers that have everything the software needs to run including libraries, system tools, code, and runtime
  (for example, dependencies). Using Docker, you can quickly deploy and scale applications into any environment and know your code will run.
  
  A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing   environment to another. For example, A Docker container image is a lightweight, standalone, executable package of software that includes everything         needed to run an application: code, runtime, system tools, system libraries and settings.
  Container images become containers at runtime.
  (*Here image refers to a computer file containing code, i.e. structure and contents of all installed tools, softwares and dependencies packed as             container*)
  
## How docker works and why it's better than Virtual machines(VMs)?
Check out this Youtube video for understanding docker and VMs: https://www.youtube.com/watch?v=u-YWtdbpEhQ&t=3s

## Docker vs Conda
  From a high level both of them provide isolated fully-configurable environments allowing developers to avoid dependency resolution on any host computers.
  Docker’s concept of a registry is the very same as a package manager, except they deal in images and Dockerfiles rather than releases and source code.

  If you’re distributing software that can run in isolation, Docker may be for you.
  Docker runs software in isolation by distributing them among different containers, while conda runs all the needed software under one enviornment which is
  basically overlaid on top of ones system.
