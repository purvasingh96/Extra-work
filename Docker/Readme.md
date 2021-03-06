# What is docker?
Docker is world's leading software container platform. What does this mean?

## Problem faced in software industry
* A typical software engineer stack consists of -
  * Front-end components
  * Back-end components
  * Databases
  * Dependencies
 * A software engineer has to make sure that all the components of a software stack should work in different kinds of platform, which in-turn creates a **matrix from hell** as shown below -
 <img src="./images/06.software_eng_problem.png"></img>

## Where does Docker come into picture?
* We have the following steps involved in a typical software development life-cycle. Docker comes at the **deployment stage.**<br>
<img src="./images/07.docker_operation_stage.png"></img>

## How does docker help to solve matrix from hell problem?
### Problems faced in Software Industry v/s Shipping Industry 
The problem faced by software engineers is very similar to what people from shipping industry faced a long time ago.<br> They had to ship various goods that belonged to different categories for ex. some were liquid, some were solid, some had different shapes and sizes etc. Their matrix from hell looked something like below - <br>
<img src="./images/05.shipping_industry_problem.png"></img><br>
## How did shipping industry solve their problem?
They switched to using **containers**, where goods can be manufactured as per standards.<br>
<img src="./images/04.shipping_industry_solved.png"></img><br>
## How did software engineers solve their problem?
Software engineers resorted to something similar, i.e. they used **docker containers**. Docker container allows a developer to package up an application with all the parts it needs, such as libraries and other dependencies and ship it out as one package.<br>
<img src="./images/01.sw_problem_solved.png"></img><br>

# Docker Workflow
The below image describes the workflow of how docker works. Below is the description of every component -
1. Developer creates a **Dockerfile** where she lists all the dependencies of her application. 
2. A **Dockerfile** describes all the steps to create a **Docker image.** Docker images are template used to create docker containers. Container is running instance of image.
3. When you run a Docker image, you get a **Docker container**. Docker container has application with all its dependencies.
4. Run-time instances of Docker image can be stored on an online cloud platform - [Docker Hub](https://hub.docker.com/)
5. These images can be pulled to create containers in any environment.<br>
<img src="./images/02.docker_workflow.png"></img><br>

# Components of Docker
<img src="./images/10.docker_components.png"></img><br>

# Containerization v/s Virtualization
| Containerization                                                                                                                                                                       | Virtualization                                    |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|
| Containerization is a lightweight alternative to full machine <br> virtualization that involves encapsulating your application in a <br> container with its own operating environment. | A virtual machine is a copy of a complete server. |
| Represents OS virtualization                                                                                                                                                           | Reperesents hardware level virtualization         |
| Real-time provisioning and scaling                                                                                                                                                     | Slow provisioning                                 |
| Native performance                                                                                                                                                                     | Limited performance                               |
| Process-level isolation, hence less secure.               | Fully isolated, hence more secure.                | 

<br>
<img src="./images/03.virtualization_vs_containerization.png"></img><br>

# Benifits of Docker
* **Build your application only once**
  * An application inside container can run on any system that has Docker installed. Therefore, no need to configure app multiple times for various platforms.
* **Testing application inside container**
  * In Docker, you test your application inside docker container, hence the testing result that you recieved in test environment, would be the same you would get in production environment as well, as they would be running same docker container.
* **Easy portability**
  * If you created your container using amazon EC2 machine, you can then port this machine to virtual box and it will run as it is.
* **Easy version controlling**
  * Just like GIT, if you make any changes in your image, you can easily commit those changes and create new version.
* **Application encapsulation/isolation**
  * Every application runs inside its own container and does not interfere with other running applications.
* **Easy deployments**
* **Docker simplifies DevOps**





