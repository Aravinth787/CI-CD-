# CI-CD-PIPELINE


# CI/CD Pipeline with Jenkins

This repository demonstrates a Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins. The pipeline automates the process of building, testing, and deploying the application.

## Table of Contents

- [Overview](#overview)
- [Pre-requisites](#pre-requisites)
- [Jenkins Pipeline](#jenkins-pipeline)
- [Setup Instructions](#setup-instructions)
  - [Step 1: Install Jenkins](#step-1-install-jenkins)
  - [Step 2: Install Required Plugins](#step-2-install-required-plugins)
  - [Step 3: Configure Jenkins](#step-3-configure-jenkins)
  - [Step 4: Create Jenkinsfile](#step-4-create-jenkinsfile)
  - [Step 5: Set Up Webhook (Optional)](#step-5-set-up-webhook-optional)
  - [Step 6: Execute the Pipeline](#step-6-execute-the-pipeline)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Overview

The CI/CD pipeline automates the process of integrating code changes, testing, and deploying the application. This project uses Jenkins, an open-source automation server, to manage and run the pipeline.

### Key Features

- **Continuous Integration:** Automatically build and test code on each commit.
- **Continuous Deployment:** Automatically deploy the application after passing tests.
- **Version Control:** GitHub is used for version control.
- **Automated Tests:** Ensure that code quality is maintained by running tests.

## Pre-requisites

Before setting up the Jenkins pipeline, ensure you have the following:

- **Jenkins:** Installed and running on your server.
- **Git:** Installed and configured on your Jenkins server.
- **GitHub Repository:** The repository containing your project.

## Jenkins Pipeline

The Jenkins pipeline is defined using a `Jenkinsfile` in the root of your repository. This file includes stages for building, testing, and deploying the application.



## Setup Instructions

### Step 1: Install Jenkins

- Follow the [official Jenkins installation guide](https://www.jenkins.io/doc/book/installing/) to install Jenkins on your server.

### Step 2: Install Required Plugins

- Go to **Manage Jenkins > Manage Plugins** and install the following plugins:
  - Git Plugin
  - Pipeline Plugin
  - GitHub Integration Plugin

### Step 3: Configure Jenkins

- Set up Jenkins to pull the code from your GitHub repository:
  1. Go to **Manage Jenkins > Configure System**.
  2. Add GitHub Server details under the GitHub section.

### Step 4: Create Jenkinsfile

- Create a `Jenkinsfile` in the root directory of your project with the necessary stages for build, test, and deploy.

### Step 5: Set Up Webhook (Optional)

- Set up a webhook in GitHub to trigger the Jenkins pipeline on every commit:
  1. Go to your repository on GitHub.
  2. Navigate to **Settings > Webhooks**.
  3. Add a new webhook with the Jenkins URL and `/github-webhook/` as the endpoint.

### Step 6: Execute the Pipeline

- Go to Jenkins and create a new Pipeline project.
- Link it to your GitHub repository and trigger the build manually or through the webhook.

## Troubleshooting

- **Build Failures:** Check the console output in Jenkins for detailed error messages.
- **Webhook Issues:** Ensure that Jenkins is accessible from the internet if using webhooks.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for any bugs or feature request

## Here is the output for CI/CD Pipeline Using Jenkins


![PIPELINE](https://github.com/user-attachments/assets/c936c10d-5a0d-495a-a731-b194371cfccd)

