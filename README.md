created a Weather-App in Nodejs to run in Docker containerized
******************************************************************************************************************************
- Required A EC2 instances in aws cloud of single machine
- second one - install jenkins & openjdk 17 
         
         sudo apt update
         sudo apt upgrade
         sudo apt install openjdk-17-jdk
         sudo apt install openjdk-17-jre
    sudo apt-get update
    sudo apt-get install jenkins
- after comletion. so need a docker in ubuntu
   install a docker in ubuntu
- go to jenkins
   - required a some plugins for docker registry authentication
   - Write a Declarative Pipeline in jenkins pipeline project
   - added 4 to 5 stages in that jenkins pipeline.
   - configure a global account to add git & docker credentials in that with tools configuration.
- CI - continuos integration
    - Git Checkout
    - Docker Build Image
    - Docker Push Image - in Docker Hub
    - Docker Pull Image from Docker Hub
- CD - Continous Delivery or Deployement
    - Deploye A NodeJS Project of Weather_App in Docker Containerisation
    - do to run app in docker container of expose 3000.
 
 
 ***************************************************************************************************************************************************************************************
 Final Output 
  - to check in browser. /127.0.0.1:3000

    ![image](https://github.com/vivek2021-dot/Weather_App/assets/88077049/f8ab1c07-4b9d-4d61-9c35-34b585422b72)

      
    
