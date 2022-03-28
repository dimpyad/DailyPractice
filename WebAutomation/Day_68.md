### Learning Goal
Run tests on container - Parallel Execution

### Steps to automate
1. Open any website on <chrome> browser
2. Add a simple validation
3. Execute the steps 1 and 2 parallelly on <firefix> browser 

### Problem statement
- Run the above tests on a docker container running in local machine.

### Prerequisites and steps to follow
- Setting up Docker (https://docs.docker.com/engine/install/)
- Pull the docker image selenium/standalone-chrome 
- Pull the docker image - selenium/standalone-firefox
- Run the Selenium Webdriver Docker container
- Create a simple selenium tests using Remote web driver and run the tests parallelly on two browsers.
