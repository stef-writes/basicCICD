Learning-by-Doing Task: Implementing a Basic CI/CD Pipeline
Context: This week's lecture introduced the fundamental concepts of Continuous Integration
(CI), Continuous Delivery (CD), and the importance of Infrastructure as Code (IaC) in modern
DevOps practices. You learned about automating the software development lifecycle to improve
efficiency, reduce errors, and accelerate the delivery of software.
Objective: This task aims to solidify your understanding of CI/CD principles and Infrastructure
as Code by setting up a basic pipeline for a simple application. You will practice automating the
build, test, and deployment stages.
Task Breakdown:
Part 1: Infrastructure as Code (IaC)
(Focus: Defining and Provisioning Infrastructure)
1. Choose an IaC Tool: Select one of the following tools to define your infrastructure:
●
Vagrant: (Good for local development environments)
●
Docker Compose: (If you are comfortable with containerization)
●
(Optional, if you have prior experience): AWS CloudFormation (for cloud-based
infrastructure)*
2. Define Your Infrastructure: Create an IaC configuration file (e.g., Vagrantfile,
docker-compose.yml) that describes a basic environment for a simple web
application. This environment should include:
●
One virtual machine/container: Specify the operating system (e.g., Ubuntu) or
base image.
●
A web server: Specify the web server to be installed (e.g., Nginx, Apache). You
don't need to deploy a full application yet.
3. Provision Your Infrastructure: Use your chosen IaC tool to create the environment
defined in the previous step.
4. Verify the Infrastructure: Once provisioned, access the web server (e.g., by navigating
to http://localhost or the VM's IP address in your browser) and ensure the default
web server page is displayed.
Part 2: Continuous Integration (CI)
(Focus: Automating Build and Test)
1. Create a Simple Application: Write a very basic "Hello, World!" web application. This
can be in any language you are comfortable with (e.g., Python Flask, Node.js Express, a
simple HTML file).
2. Initialize a Git Repository: Create a local Git repository for your application.
3. Choose a CI Tool: Select one of the following CI tools:
●
GitHub Actions: (If you are using GitHub for your repository)
●
GitLab CI/CD: (If you are using GitLab)
●
(Optional, if you have prior experience): Jenkins (requires installation)*
4. Define Your CI Pipeline: Create a CI configuration file (e.g.,
.github/workflows/main.yml, .gitlab-ci.yml) that defines the following
stages:
●
Checkout: Retrieve your application code from the Git repository.
●
Build: Install any necessary dependencies for your application. For example, if
using Python, this might involve running pip install -r
requirements.txt.
●
Test: Add a simple test to verify your application is working (e.g., a basic HTTP
request to your application's endpoint that returns a 200 OK status).
5. Commit and Push Your Code: Commit your application code and CI configuration file
to your Git repository and push it to the remote repository.
6. Trigger the CI Pipeline: Observe your CI tool automatically trigger the pipeline upon
your code push.
7. Review the CI Results: Examine the logs and results of each stage in your CI pipeline
to ensure they passed successfully.
Part 3: Continuous Delivery (CD)
(Focus: Automating Deployment)
1. Extend Your CI Pipeline for CD: Modify your CI configuration file to add a Deploy
stage that is triggered after the Test stage is successful.
2. Automate Deployment: Within the Deploy stage, add steps to automatically deploy
your simple application to the infrastructure you provisioned in Part 1. This might involve:
●
If using Vagrant: Use a provisioning script within your Vagrantfile to copy
your application files to the VM and configure the web server to serve them.
●
If using Docker Compose: Build a Docker image of your application and
update your docker-compose.yml to include your application container.
●
(Optional, if using AWS): Utilize AWS CLI commands to deploy your
application to an EC2 instance or a container service.
3. Verify the Deployed Application: Once the CD pipeline has completed successfully,
access your application in your browser using the appropriate URL or IP address for
your provisioned environment. You should see your "Hello, World!" application.
Deliverables:
For each part, submit the following:
Part 1: Infrastructure as Code (IaC)
●
The IaC configuration file you created (e.g., Vagrantfile, docker-compose.yml).
●
A screenshot showing the default web server page running in your provisioned
environment.
Part 2: Continuous Integration (CI)
●
The source code for your simple web application.
●
The CI configuration file you created (e.g., .github/workflows/main.yml,
.gitlab-ci.yml).
●
A screenshot of your CI tool showing a successful pipeline run.
Part 3: Continuous Delivery (CD)
●
The updated CI configuration file with the deployment stage.
●
A brief explanation of how you automated the deployment process.
●
A screenshot of your deployed "Hello, World!" application running in your provisioned
environment.
Bonus Challenge:
●
Implement Basic Monitoring: Add a basic monitoring solution (e.g., using top or htop
within your VM/container or a simple ping check) to your CI/CD pipeline to verify the
health of your deployed application.
Submitting Your Work:
Organize your code, configuration files, screenshots, and explanations for each part into a
single document (e.g., a Word document or PDF). Submit this document as instructed by your
instructor.