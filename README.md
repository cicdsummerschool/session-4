# Session 4: A Closer Look at Canary Deployments

Homework for this session consists of reading a classic document on canary deployments and working through (or at least reading through) labs on implementing caranry deployments on Google Cloud Platform (GCP) and Amazon Elastic Container Service (ECS).

## [Canary Release by Danilo Santos, Thoughtworks](https://martinfowler.com/bliki/CanaryRelease.html)

The article explains the concept of a Canary Release, a strategy for minimizing risk when deploying new software versions. It involves gradually rolling out the update to a small subset of users before full deployment. This method allows for real-time monitoring and quick rollback if issues arise, making it a safer alternative to deploying across the entire infrastructure at once. The article also discusses strategies like using Phoenix or Immutable Servers and highlights challenges such as managing multiple software versions simultaneously.

- Full article [here](https://martinfowler.com/bliki/CanaryRelease.html).

## [Cloud Run Canary Deployments](https://www.cloudskillsboost.google/focuses/52827?parent=catalog)

In this lab you will learn how to implement a deployment pipeline for Cloud Run that executes a progression of code from developer branches to production with automated canary testing and percentage based traffic management. It is intended for developers and DevOps engineers who are responsible for creating and managing CI/CD pipelines to Cloud Run.

_Note: The content in this lab is associated with the Cloud Skills Boost service.  However, you don't have to pay for the service to follow along with the instructions; you just need your own GCP account._

- If you aren't able to access the content from the link above, a PDF copy of the lab is available here: [Cloud Run Canary Deployments PDF](./cloud-run-canary-deployments-google-cloud.pdf)

## [Blue/Green Deployments :: Amazon ECS Workshop](https://ecsworkshop.com/blue_green_deployments/)

The article from the Amazon ECS Workshop explains Blue/Green Deployments, a method for deploying applications by shifting traffic between two identical environments (Blue and Green) running different versions of the same application. This approach allows for validation of the new version (Green) while keeping the old version (Blue) live, ensuring minimal risk and easy rollback if issues arise. This technique is particularly useful for critical workloads where downtime or impaired operation must be minimized.

- Full article [here](https://ecsworkshop.com/blue_green_deployments/).

## [Deploying an Amazon ECS service using a blue/green deployment](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-blue-green.html)

The AWS documentation provides a detailed guide on implementing Blue/Green Deployments using Amazon ECS and AWS CodeDeploy. It walks through setting up the necessary infrastructure, including load balancers, ECS clusters, and task definitions. The guide also covers the creation of deployment groups and CodeDeploy resources, and how to monitor and manage the deployment process. It ends with instructions on cleaning up resources to avoid unnecessary charges. This comprehensive guide ensures a smooth and controlled deployment process with minimal risk.

- Full article [here](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-blue-green.html).
