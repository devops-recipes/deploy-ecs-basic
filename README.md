# Deploy a Node.js application to Amazon ECS

[![Run Status](https://api.shippable.com/projects/58f6fcddd1780a07007bba3f/badge?branch=master)](https://app.shippable.com/github/devops-recipes/deploy-ecs-basic) [![Coverage Badge](https://api.shippable.com/projects/58f6fcddd1780a07007bba3f/coverageBadge?branch=master)](https://app.shippable.com/github/devops-recipes/deploy-ecs-basic)

![AyeAye](https://github.com/devops-recipes/deploy-ecs-basic/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha and istanbul. It also does a docker build once CI passes and then pushes the image to Amazon EC2 Container Registry

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](wwww.shippable.com)
* Create an [integration](http://docs.shippable.com/platform/integration/aws-keys/) on shippable to your Amazon ECR
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `dr-aws-keys`
* Change the ECR_REPO to point to your repo
* You should be able to run a manual build or webhook build on commit

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/devops-recipes/deploy-ecs-basic/blob/master/public/resources/images/integration-creation.png)

### CI Console Output
![CI Console Output](https://github.com/devops-recipes/deploy-ecs-basic/blob/master/public/resources/images/console.jpg)
