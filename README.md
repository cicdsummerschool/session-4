# Session 4: A Closer Look at Canary Deployments

Homework for this session consists of reading a classic document on canary deployments and working through (or at least reading through) a couple labs on using Blue-Green deployments with Amazon Elastic Container Service (ECS).

## [Canary Release by Danilo Santos, Thougtworks](https://martinfowler.com/bliki/CanaryRelease.html)

The article by Martin Fowler explains the concept of a Canary Release, a strategy for minimizing risk when deploying new software versions. It involves gradually rolling out the update to a small subset of users before full deployment. This method allows for real-time monitoring and quick rollback if issues arise, making it a safer alternative to deploying across the entire infrastructure at once. The article also discusses strategies like using Phoenix or Immutable Servers and highlights challenges such as managing multiple software versions simultaneously.

- Full article [here](https://martinfowler.com/bliki/CanaryRelease.html).


## [Blue/Green Deployments :: Amazon ECS Workshop](https://ecsworkshop.com/blue_green_deployments/)

The article from the Amazon ECS Workshop explains Blue/Green Deployments, a method for deploying applications by shifting traffic between two identical environments (Blue and Green) running different versions of the same application. This approach allows for validation of the new version (Green) while keeping the old version (Blue) live, ensuring minimal risk and easy rollback if issues arise. This technique is particularly useful for critical workloads where downtime or impaired operation must be minimized.

- Full article [here](https://ecsworkshop.com/blue_green_deployments/).

## [Deploying an Amazon ECS service using a blue/green deployment](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-blue-green.html)

The AWS documentation provides a detailed guide on implementing Blue/Green Deployments using Amazon ECS and AWS CodeDeploy. It walks through setting up the necessary infrastructure, including load balancers, ECS clusters, and task definitions. The guide also covers the creation of deployment groups and CodeDeploy resources, and how to monitor and manage the deployment process. It ends with instructions on cleaning up resources to avoid unnecessary charges. This comprehensive guide ensures a smooth and controlled deployment process with minimal risk.

- Full article [here](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-blue-green.html).
