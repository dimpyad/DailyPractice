### Learning Goal
Run tests on container - Create docker file

### Steps to automate
1. Open any website on <chrome> browser
2. Add a simple validation
3. Execute the steps 1 and 2 parallelly on <firefix> browser 

### Problem statement
- Add a docker file into your test code which will perform all the necessary things in side a docker container to run the selenium tests. The following dependencies should be installed in the docker container:
  1. java
  2. maven
  3. Browser drivers
  4. Coping the code to working directory

### Prerequisites and steps to follow
- Setting up Docker (https://docs.docker.com/engine/install/)
- Pull the docker image selenium/standalone-chrome 
- Pull the docker image - selenium/standalone-firefox
- Run the Selenium Webdriver Docker container
- Create a simple selenium tests using Remote web driver and run the tests parallelly on two browsers.
- Install Jenkins on your local machine (https://www.jenkins.io/doc/book/installing/
- Add job in Jenkins which will take latest code from git and build and execute the tests on the docker container in local selenium grid.
  
### References
- https://medium.com/@ahamedabdulrahman/dockerize-selenium-java-project-and-run-selenium-scripts-within-docker-container-c2603d1bac3f

