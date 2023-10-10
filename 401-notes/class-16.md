# Class 16 Notes

## Reading

### AWS EC2

What is an EC2 Instance?

- It is an Elastic Compute Cloud instance is a virtual server in Amazon Web Services that provides scalable computing capacity in the cloud. It allows users to run applications and host services on virtual machines with various configurations.

Name 2 use cases for EC2.

- Web hosting and data processing

Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

- ECS has more flexibility and control and allows user to orchestrate and manage Docer containers, providing more granular control over the application infrastructure and deployment process.

### EC2 For Humans

Where can we find EC2 on the AWS Console?

- You can find it under the 'Compute' section labeled as 'EC@' or 'Elastic Compute Cloud'

Explain the general difference between T2 Micro and XL.

- T2 Micro is a small, low-cost instance suitable for lightweight workloads, while EL typically denotes an extra-large instance with significantly more computing power, memory and stroage capacity.

Explain a “Compute Cycle” to a non-technical friend.

-  This worker's job is to complete one task at a time. Think of each task as something the worker needs to do, like putting together a toy or packaging a product.

Now, the worker can finish one task and move on to the next. The speed at which the worker finishes these tasks is like the worker's "compute cycle." It tells us how fast and efficiently the worker can complete each job.

In the world of computers, a compute cycle is similar. It's like a computer's worker doing tasks, but instead of toys or products, it's doing calculations, solving problems, or running software. The faster and more efficiently a computer can do these tasks, the better it performs. So, a compute cycle is like the computer's work pace – how quickly it gets things done.

### Elastic Beanstalk

What is Elastic Beanstalk?

- a Platform as a Service offering that simplifies the deployment and management of application in AWS.

Describe the relationship between EC2 and Elastic Beanstalk.

- Elastic Beanstalk runs applications on EC2 instances. It abstracts the underlying infrastructure by automatically provisioning and managing EC2 instances, load balancing, auto-scaling, and application deployment. Users provide their application code, and Elastic Beanstalk handles the rest, making it easier to deploy and manage web applications.

Name some benefits of using Elastic Beanstalk.

- Simplified deploymeny, scalability, monitoring and logging, easy integration and multiple platform support.
