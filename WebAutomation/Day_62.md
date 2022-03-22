### Learning Goal
Run tests on container

### Resources
- https://docs.docker.com/get-started/
- https://github.com/SeleniumHQ/docker-selenium#quick-start

### Steps to automate
1. Open any website on chrome browser
2. Add a simple validation

### Problem statement
- Run the above tests on a docker container running in local machine.

### Prerequisites and steps to follow
- Setting up Docker (https://docs.docker.com/engine/install/)
- Pull the docker image (docker pull selenium/standalone-chrome)
- Run the Selenium Webdriver Docker container
- Create a simple selenium tests using Remote web driver and connect to the server running in the container.

### Additional Steps
- Extend the above program by running the same on firefox driver in a docker image.

Note: This is a simple problem to apply the understanding of execution of tests on a docker container. We are going to cover more complex scenarios like cross browser testing, using selenium grid, distributing testing among multiple containers etc in upcoming challenges.
