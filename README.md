# CI-CD_with_Jenkins
![CI-CD with Jenkins Diagram](https://github.com/Asare12/CI-CD_with_Jenkins/blob/master/images/MicrosoftTeams-image__282_29.png)

## Continuous Integration
Developers merge/commit code to master branch multiple times a day, fully automated build and test process which gives feedback within few minutes, by doing so, you avoid the integration hell that usually happens when people wait for release day to merge their changes into the release branch.

## Continuous Delivery
An extension of continuous integration to make sure that you can release new changes to your customers quickly in a sustainable way. This means that on top of having automated your testing, you also have automated your release process and you can deploy your application at any point of time by clicking on a button. In continuous Delivery the deployment is completed manually.

## Continuous Deployment
Goes one step further than continuous delivery, with this practice, every change that passes all stages of your production pipeline is released to your customers, there is no human intervention, and only a failed test will prevent a new change to be deployed to production.

## How CICD Practices relate to each other
To put it simply, the continuous integration is part of both continuous delivery and continuous deployment. The main difference is the deployment step, in continuous delivery the deployment is done manually and in continuous deployment it happens automatically.

## What is a CI CD Pipeline
The CI/CD pipeline is all about automation: Initiating code builds, automated testing, and automated deploying to the staging or production environments. It’s complex and exciting at the same time, but incredibly fast, if the output of any stage fails, the next stage will also fail.

## Set up Jenkins
### setting up ssh connection Git-hub Jenkins
- Generate new ssh key in you localhost/laptop and name it yournamejenkins
- copy public ssh key in into github the .pub file yournamejenkins.pub
- copy provate ssh key int o Jenkins - yournamejenkins.pub
- add git-hub url into repository URL after select Git underneath source code managment
- add https git-hub repo url in the git project
- change the branch to main
- execute shell
```
cd app
npm install
npm test
```
- save and trigger the build
