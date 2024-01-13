"I created a Weather-App in Node.js to run in a Docker containerized environment.
*************************************************************************************************************************************************************
In the AWS cloud, it required an EC2 instance of a single machine. For the second instance, I installed Jenkins and OpenJDK 17 using the following commands:

- sudo apt update
- sudo apt upgrade
- sudo apt install openjdk-17-jdk
- sudo apt install openjdk-17-jre
- sudo apt-get update
- sudo apt-get install jenkins

After completing this, I installed Docker on Ubuntu:

sudo apt install docker

Next, in Jenkins:

- I installed some plugins for Docker registry authentication.
- I wrote a Declarative Pipeline in the Jenkins pipeline project.
- I added 4 to 5 stages in that Jenkins pipeline.
- I configured a global account to add Git and Docker credentials in the tools configuration.
- For Continuous Integration (CI), the pipeline included the following stages:

- Git Checkout
- Docker Build Image
- Docker Push Image to Docker Hub
- Docker Pull Image from Docker Hub
- For Continuous Delivery or Deployment (CD), I deployed a Node.js project of the Weather-App in Docker Containerization. The application runs in a Docker container and is exposed on port 3000.

To view the final output, check in the browser at 127.0.0.1:3000."
 
 ***************************************************************************************************************************************************************************************
    
![image](https://github.com/vivek2021-dot/Weather_App/assets/88077049/e97b0300-9672-4ac5-91a1-79155a705c00)

      
    
