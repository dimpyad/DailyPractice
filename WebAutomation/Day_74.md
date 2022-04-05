### Learning Goal
Run tests on container - run on CI environment

### Steps to automate
1. Open any website on <chrome> browser
2. Add a simple validation
3. Execute the steps 1 and 2 parallelly on <firefix> browser 
4. Push the code to github
5. Run the tests from Jenkin's job (manually and then with scheduler)


### Problem statement
- Run the above tests on a docker container running in local machine.

### Prerequisites and steps to follow
- Setting up Docker (https://docs.docker.com/engine/install/)
- Pull the docker image selenium/standalone-chrome 
- Pull the docker image - selenium/standalone-firefox
- Run the Selenium Webdriver Docker container
- Create a simple selenium tests using Remote web driver and run the tests parallelly on two browsers.
- Install Jenkins on your local machine (https://www.jenkins.io/doc/book/installing/
- Add job in Jenkins which will take latest code from git and build and execute the tests on the docker container in local selenium grid.
  
### References
- https://medium.com/@chayathilakumarai/how-to-integrate-your-selenium-project-with-jenkins-and-git-6ab9f8b492ad
