# **Devops-Question [Shubham Kumbhar]**

**Git-Hub**
https://www.atlassian.com/git/tutorials/what-is-version-control

1. **what is DevOps?**
```
Ans: DevOps is a set of software development practices that combines software development and 
information technology operations to shorten the systems development life cycle while delivering features, 
fixes, and updates frequently in close alignment with business objectives
```
  More About [Devops](https://theagileadmin.com/what-is-devops/ "Devops")

2. **why do we need DevOps?** 
```
Ans: Five reasons why the industry has been so quick to adopt DevOps principles
1. Shorter Development Cycles, Faster Innovation 
2. Reduced Deployment Failures, Rollbacks, and Time to Recover
3. Improved Communication and Collaboration
4. Increased Efficiencies
5. Reduced Costs and IT Headcount

```
3. **Mention the key aspects or principle behind DevOps?**
```
Ans:
    The key aspects or principle behind DevOps is

1. Infrastructure as code
2. Continuous deployment
3. Automation
4. Monitoring
5. Security
    
```
4. **List out some of the popular tools for DevOps?**
```
Ans:
Configuration management tools
    - Ansible 
    - CHEF 
    - CFEngine
    - Puppet 
    - SALTSTACK 
    - JUJU 
    - RUDDER
CI/CD Tools
    Jenkins
    GoCD
    Drone.io
    TeamCity
    Wercker
    Codeship
    Travis CI
    CircleCI
    Bamboo
    Gradle

Container orchestration tools
    - Kubernetes
    - Docker Swarm
    - Google Container Engine
    - Mesosphere Marathon 

version control tools
    Git
    Git hub
    Beanstalk
    Bitbucket
    PerForce
    Apache Subversion
    AWS CodeCommit
    Git-lab
    
```
5. **what is a version control system?** 
```
Ans:
A version control system allows users to keep track of the changes in software development projects, and 
enable them to collaborate on those projects. Using it, the developers can work together on code and 
separate their tasks through branches.

There can be several branches in a version control system, according to the number of collaborators. 
The branches maintain individuality as the code changes remain in a specified branch(s).

Developers can combine the code changes when required. Further, they can view the history of changes,
go back to the previous version(s) and use/manage code in the desired fashion.
    
```
6. **What is Git and explain the difference between Git and SVN?** 
```
Ans:
Git is a free, open source distributed version control system tool designed to handle everything from small to very large projects with speed and efficiency. It was created by Linus Torvalds in 2005 to develop Linux Kernel.
Git has the functionality, performance, security and flexibility that most teams and individual developers need. 
It also serves as an important distributed version-control DevOps tool.
```
**Difference between Git and SVN**
```
Git and SVN are both software. Git is SCM, source code management ,
and a distributed revision control system. SVN is a revision control and software versioning system.

One of the most notable differences when switching to Git is its speed.
Since the whole repository is stored locally on the developer’s machine, he or she can work for days with a very poor internet connection. Creating branches is lightning fast due to Git’s branch implementation.
In Git, a branch is simply a reference to a commit, where the following commits will be attached.
It doesn’t contain even basic information like create date, user who created it or some kind of a message.

Since Git encourages the use of branches, we can’t forget to give a shout-out to its merge capabilities. 
SVN before version 1.5 only did two-way merges that involved a change set applied to the current codebase, because it didn’t store merge information. Git uses the history of the repository to identify the common base between the merged branches and only needs to merge from where they diverged — thereby completing a three-way merge.
SVN is also improving and has supported three-way merging since 1.5. In the upcoming 1.9 version of SVN, it will also have better rename/move tracking of files, something that Git already does.

    
```

7. **what language is used in Git?** 
```
Ans:
    Git’s Source code is hosted on Github here: git/git

So, From that these are the languages used in that repository:

C - 45%
Shell - 35%
Perl - 8%
Tcl - 5%
Python - 2%
C ++ - 2%
    
```
 [GIT-Source Code](https://github.com/git/git "GIT-Source Code")

8. **what are the advantages and disadvantages of using Git?**
```
Ans:
GIT is a distributed version control system and source code management system with an emphasis to
handle small and large projects with speed and efficiency.

let’s start with advantages :

Data redundancy and replication
- High availability
- Only one.git directory per repository
- Superior disk utilization and network performance
- Collaboration friendly
- Any sort of projects can use GIT

There are very few disadvantages of using GIT:

- Git is less preferred for handling extremely large files or frequently changing binary files .

- GIT does not support ‘commits’ across multiple branches or tags.

    
```

9. **Explain the difference between git pull and git fetch?** 

```
Ans:
    Before we talk about the differences between these two commands,
    let's stress their similarities: both are used to download new data from a remote repository.

->  Downloading data is an essential step in your daily work - because the remote data you are looking at in your local repository is just a "snapshot". 
It's only as up-to-date as the last time you explicitly downloaded fresh data from the remote with "fetch" or "pull".
It's vital to keep this fact in mind when inspecting remote branches and commits!

Let's now look at the fine but important differences between "fetch" and "pull".


    Fetch
                $ git fetch origin


->  git fetch really only downloads new data from a remote repository - 
but it doesn't integrate any of this new data into your working files. 
Fetch is great for getting a fresh view on all the things that happened in a remote repository.

->  Due to it's "harmless" nature, you can rest assured: 
fetch will never manipulate, destroy, or screw up anything. This means you can never fetch often enough.

    Pull
            $ git pull origin master

-> git pull, in contrast, is used with a different goal in mind:
to update your current HEAD branch with the latest changes from the remote server.
This means that pull not only downloads new data;
it also directly integrates it into your current working copy files. 
This has a couple of consequences:

-> Since "git pull" tries to merge remote changes with your local ones, a so-called "merge conflict" can occur.
Check out our in-depth tutorial on How to deal with merge conflicts for more information.

-> Like for many other actions, it's highly recommended to start a "git pull" only with a clean working copy.
This means that you should not have any uncommitted local changes before you pull. 
Use Git's Stash feature to save your local changes temporarily.
```
10. **what is Docker?**
```
Ans:
Docker is a tool designed to make it easier to create, deploy, and run applications by using containers. 
Containers allow a developer to package up an application with all of the parts it needs,
such as libraries and other dependencies, and ship it all out as one package. 
By doing so, thanks to the container, the developer can rest assured that the application will run on any 
other Linux machine regardless of any customized settings that machine might have that could differ from the machine used for writing and testing the code.
    
```
11. **what is Docker image?**
```
Ans:

A Docker image is made up of multiple layers. A user composes each Docker image to include system libraries, tools, and other files and dependencies for the executable code. 
Image developers can reuse static image layers for different projects. Reuse saves time, because a user does not have to create everything in an image.

Most Docker images start with a base image, although a user can build one entirely from scratch, if desired.
Each image has one readable/writable top layer over static layers.
Layers are added to the base image to tailor the code to run in a container. 
Each layer of a Docker image is viewable under /var/lib/docker/aufs/diff, or via the Docker history command in the command line interface (CLI). By default, Docker shows all top-layer images, such as the repository, tags and file sizes. 
Intermediate layers are cached, which makes top layers easier to view. 
Docker utilizes storage drivers to manage contents of image layers.

When a new container is created from an image, a writable layer is also created. 
This layer is called the container layer, and it hosts all changes made to the running container.
This layer can store newly written files, modifications to existing files and newly deleted files.
The writable layer allows customization of the container.
Changes made to the writable layer are saved on that layer. 
Multiple containers can share the same underlying base image and have their own data state thanks to the writable layer.
    
```
12. **what is Docker Container?**
```
Ans:

Package Software into Standardized Units for Development, Shipment and Deployment
A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.
A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

Container images become containers at runtime and in the case of Docker containers - images become containers when they run on Docker Engine. Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure. Containers isolate software from its environment and ensure that it works uniformly despite differences for instance between development and staging.

Docker containers that run on Docker Engine:

Standard: Docker created the industry standard for containers, so they could be portable anywhere
Lightweight: Containers share the machine’s OS system kernel and therefore do not require an OS per application, driving higher server efficiencies and reducing server and licensing costs
Secure: Applications are safer in containers and Docker provides the strongest default isolation capabilities in the industry
    
```
13. **What are the components of Docker Architecture and explain?**
```
Ans:
Docker Client
The Docker client enables users to interact with Docker. The Docker client can reside on the same host as the daemon or connect to a daemon on a remote host. A docker client can communicate with more than one daemon. 
The Docker client provides a command line interface (CLI) that allows you to issue build, run, and stop application commands to a Docker daemon.

The main purpose of the Docker Client is to provide a means to direct the pull of images from a registry and to have it run on a Docker host. Common commands issued by a client are:

docker build
docker pull
docker run
DockerHost
The Docker host provides a complete environment to execute and run applications.
It comprises of the Docker daemon, Images, Containers, Networks, and Storage. As previously mentioned, the daemon is responsible for all container-related actions and receives commands via the CLI or the REST API. 
It can also communicate with other daemons to manage its services.
The Docker daemon pulls and builds container images as requested by the client. Once it pulls a requested image, it builds a working model for the container by utilizing a set of instructions known as a build file. The build file can also include instructions for the daemon to pre-load other components prior to running the container, or instructions to be sent to the local command line once the container is built.

Docker Objects
Various objects are used in the assembling of your application. The main requisite Docker objects are:


Images
Images are a read-only binary template used to build containers.
Images also contain metadata that describe the container's capabilities and needs. Images are used to store and ship applications. 
An image can be used on its own to build a container or customized to add additional elements to extend the current configuration. Container images can be shared across teams within an enterprise using a private container registry, or shared with the world using a public registry like Docker Hub.
Images are a core part of the Docker experience as they enable collaboration between developers in a way that was not possible before.


Containers
Containers are encapsulated environments in which you run applications. The container is defined by the image and any additional configuration options provided on starting the container, including and not limited to the network connections and storage options. Containers only have access to resources that are defined in the image, unless additional access is defined when building the image into a container. You can also create a new image based on the current state of a container. Since containers are much smaller than VMs, they can be spun up in a matter of seconds, and result in much better server density.


Networking
Docker implements networking in an application-driven manner and provides various options while maintaining enough abstraction for application developers. There are basically two types of networks available - the default Docker network and user-defined networks. By default, you get three different networks on the installation of Docker - none, bridge, and host. The none and host networks are part of the network stack in Docker. The bridge network automatically creates a gateway and IP subnet and all containers that belong to this network can talk to each other via IP addressing. This network is not commonly used as it does not scale well and has constraints in terms of network usability and service discovery.

The other type of networks is user-defined networks. Administrators can configure multiple user-defined networks. There are three types:

Bridge network: Similar to the default bridge network, a user-defined Bridge network differs in that there is no need for port forwarding for containers within the network to communicate with each other. The other difference is that it has full support for automatic network discovery.
Overlay network: An Overlay network is used when you need containers on separate hosts to be able to communicate with each other, as in the case of a distributed network. However, 
a caveat is that swarm mode must be enabled for a cluster of Docker engines, known as a swarm, to be able to join the same group.
Macvlan network: When using Bridge and Overlay networks a bridge resides between the container and the host. A Macvlan network removes this bridge, providing the benefit of exposing container resources to external networks without dealing with port forwarding. This is realized by using MAC addresses instead of IP addresses.

Storage
You can store data within the writable layer of a container but it requires a storage driver. Being non-persistent, it perishes whenever the container is not running. Moreover, it is not easy to transfer this data. In terms of persistent storage, Docker offers four options:

Data Volumes: Data Volumes provide the ability to create persistent storage, with the ability to rename volumes, list volumes, and also list the container that is associated with the volume. Data Volumes sit on the host file system, outside the containers copy on write mechanism and are fairly efficient.
Data Volume Container: A Data Volume Container is an alternative approach wherein a dedicated container hosts a volume and to mount that volume to other containers. In this case, the volume container is independent of the application container and therefore can be shared across more than one container.
Directory Mounts: Another option is to mount a host’s local directory into a container. In the previously mentioned cases, the volumes would have to be within the Docker volumes folder, whereas when it comes to Directory Mounts any directory on the Host machine can be used as a source for the volume.
Storage Plugins: Storage Plugins provide the ability to connect to external storage platforms. These plugins map storage from the host to an external source like a storage array or an appliance. A list of storage plugins can be found on Docker’s Plugin page.


Storage Plugins
There are storage plugins from various companies to automate the storage provisioning process. For example, 
HPE 3PAR
EMC (ScaleIO, XtremIO, VMAX, Isilon)
NetApp
There are also plugins that support public cloud providers like:

Azure File Storage
Google Compute Platform.
Docker Registries
Docker registries are services that provide locations from where you can store and download images. In other words, a Docker registry contains repositories that host one or more Docker Images. Public Registries include Docker Hub and Docker Cloud and private Registries can also be used. Common commands when working with registries include:

docker push
docker pull
docker run

Service Discovery
Service Discovery allows containers to find out about the environment they are in and find other services offered by other containers.

It is an important factor when trying to build scalable and flexible applications.
    
```

14. **What is the lifecycle of Docker Container?**
```
Ans:

** Create container

Create a container to run it later on with required image.

docker create --name <container-name> <image-name>
Run docker container
Run the docker container with the required image and specified command / process. ‘-d’ flag is used for running the container in background.

docker run -it -d --name <container-name> <image-name> bash

 
** Pause container
Used to pause the processes running inside the container.

docker pause <container-id/name>

**Unpause container
Used to unpause the processes inside the container.

docker unpause <container-id/name>

**Start container
Start the container, if present in stopped state.

docker start <container-id/name>


**Stop container
To stop the container and processes running inside the container:

docker stop <container-id/name>
To stop all the running docker containers

docker stop $(docker ps -a -q)

**Restart container
It is used to restart the container as well as processes running inside the container.

docker restart <container-id/name>

**Kill container
We can kill the running container.

docker kill <container-id/name>


**Destroy container
Its preferred to destroy container, only if present in stopped state instead of forcefully destroying the running container.

docker rm <container-id/name>
To remove all the stopped docker containers

docker rm $(docker ps -q -f status=exited)

    
```

15. **Explain what is continuous integration?**
```
Ans:
    Continuous Integration (CI) is a development practice where developers integrate code into a shared repository frequently, preferably several times a day. Each integration can then be verified by an automated build and automated tests. While automated testing is not strictly part of CI it is typically implied.

One of the key benefits of integrating regularly is that you can detect errors quickly and locate them more easily. As each change introduced is typically small, pinpointing the specific change that introduced a defect can be done quickly.

In recent years CI has become a best practice for software development and is guided by a set of key principles. Among them are revision control, build automation and automated testing.

Additionally, Continuous Deployment and Continuous Delivery have developed as best-practices for keeping your application deployable at any point or even pushing your main codebase automatically into production whenever new changes are brought into it. This allows your team to move fast while keeping high quality standards that can be checked automatically.

Continuous Integration doesn’t get rid of bugs, but it does make them dramatically easier to find and remove.

-->  Continuous Integration brings multiple benefits to your organization:

1.Say goodbye to long and tense integrations
2.Increase visibility enabling greater communication
3.Catch issues early and nip them in the bud
4.Spend less time debugging and more time adding features
Build a solid foundation
Stop waiting to find out if your code’s going to work
Reduce integration problems allowing you to deliver software more rapidly

```

16. **what is a Jenkins Pipeline?**
```
Ans:
In Jenkins, a pipeline is a group of events or jobs which are interlinked with one another in a sequence.

In simple words, Jenkins Pipeline is a combination of plugins that support the integration and implementation of continuous delivery pipelines using Jenkins. A pipeline has an extensible automation server for creating simple or complex delivery pipelines "as code," via pipeline DSL (Domain-specific Language).

```


17. **What is the difference between Maven, Ant and Jenkins?**
```
Ans:
To Start with all four e.g. ANT, Maven, Jenkins and Hudson are tools to help Java developers on build, unit testing, continuous integration and project management.

Main difference between ANT and Maven is that in ANT you need to define every thing i.e. source directory, build directory, target directory etc while Maven adopts principle of Convention over configuration.

Maven also provides dependency management, standard project layout and project management. Maven has predefined project structure i.e. standard directory for source files, test files and resources.

On the other hand, Jenkins and Hudson are Continuous Integration tool, which gives you power to automate your build and deployment process. By using Jenkins or Hudson you can trigger build whenever developer commit code, to see if project is compiling fine, to run unit tests, to create build or even deploy in production or testing environment.
    
```
=====================================

18. **What is Scrum?**
```
Ans:
    Scrum is a framework within which people can address complex adaptive problems, while productively and creatively delivering products of the highest possible value.

Scrum itself is a simple framework for effective team collaboration on complex products.  Scrum co-creators Ken Schwaber and Jeff Sutherland have written The Scrum Guide to explain Scrum clearly and succinctly.  This Guide contains the definition of Scrum. This definition consists of Scrum’s roles, events, artifacts, and the rules that bind them together. 

Scrum is:

Lightweight
Simple to understand
Difficult to master
    
```


**what is Continuous Integration**

```
Continuous Integration (CI) is the process of automating the build and testing of code every 
time a team member commits changes to version control. 
```
**What is the difference between Maven, Ant and Jenkins?**

```
In short, though Maven and ANT are build tool but main difference is that maven also provides dependency management, 
standard project layout and project management. On difference between Maven, ANT and Jenkins, 
later is a continuous integration tool which is much more than build tool. 

```
**What is the relation between Hudson and Jenkins?**

```
There is no such difference between Jenkins and Hudson. Jenkins is actually the renamed version of Hudson. 
After disagreements between Oracle and Hudson creators, the latter decided that Hudson was to be forked and become Jenkins CI. 

```

**What are the advantages of Jenkins?**

```
1It is open source and it is user-friendly, easy to install and does not require additional installations or components.
2It is free of cost.
Easily Configurable. Jenkins can be easily modified and extended. It deploys code instantly, generates test reports. 
3Jenkins can be configured according to the requirements for continuous integrations and continuous delivery.

```
**Which SCM tools does Jenkins supports**

```
It supports version control tools, including AccuRev, CVS, Subversion, Git, Mercurial, 
Perforce, TD/OMS, ClearCase and RTC, and can execute Apache Ant, Apache Maven 
Platform Independent. Jenkins is available for all platforms and different operating systems, whether OS X, Windows or Linux.
Jenkins has now got a life of his own and so does Hudson.

```

**Explain about from Continuous Delivery.**
```
Continuous Delivery will explain each and every phase involved in it, such as Build, Test etc
Continuous delivery is the ability to deliver software that can be deployed at any time through manual releases; 
this is in contrast to continuous deployment which uses automated deployments. 

Success factor for the Continuous Integration
1. AUTOMATIC BUILD/DEPLOYMENT SCRIPT
2. LABELING OF ANY STABLE BUILD
3. STABILITY CRITERIA
```

**What is Configuration Management?**
```
Configuration management (CM) is a systems engineering process for establishing and maintaining consistency of a product's
performance, functional, and physical attributes with its requirements, design, and operational information throughout its life.

```



**Parameter	Agile	DevOps**
**What is it?**
1.Agile refers to an iterative approach which focuses on collaboration,
 customer feedback, and small, rapid releases.
	
DevOps is considered a practice of bringing development and operations teams together.

2.Purpose	Agile helps to manage complex projects.	

DevOps central concept is to manage end-to-end engineering processes.

3.Task	Agile process focusses on constant changes.

DevOps focuses on constant testing and delivery.

4.Team size	Small Team is at the core of Agile. As smaller is the team, the fewer people on it, the faster they can move.	

Relatively larger team size as it involves all the stack holders.

5.Feedback	Feedback is given by the customer.	

Feedback comes from the internal team.


DevOps Engineer Roles and Responsibilities:
Test, build, design, deployment, and ability to maintain the continuous integration and 
continuous delivery process using tools like Jenkins, maven Git, etc. ... 
Ability to automate test and deploy the code and monitor.

