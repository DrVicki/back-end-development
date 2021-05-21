# What is serverless with Java?

### Java remains one of the most popular languages for developing enterprise applications. Why are serverless developers leaning away from it?

May 21, 2021 | Dr. Vicki Bealman

For many years, enterprises have developed business-critical applications on diverse platforms, including physical servers, virtual machines, and cloud environments. The thing these applications have in common across industries, is they need to be continuously available (24x7x365) to guarantee stability, reliability, and performance, regardless of demand. Therefore, every enterprise must be responsible for the high costs of maintaining an infrastructure (e.g., CPU, memory, disk, networking, etc.) even if actual resource utilization is less than 50%.

Serverless architecture was developed to solve these problems. 
- Serverless permits developers to build and run applications on demand, while guaranteeing high availability without having to manage servers in multi- and hybrid-cloud environments. 
- Behind the doors, there are still many servers in the serverless topology, but they are abstracted away from application development. 
  - Instead; cloud providers use serverless services for resource management, such as provisioning, maintaining, networking, and scaling server instances.

Because of its effectiveness, the serverless development model is now a requirement for enterprises who want to spin up business applications on demand versus running them continuously.

Many open source projects have been created to manage serverless applications on [Kubernetes](https://opensource.com/article/19/6/reasons-kubernetes) clusters with the Linux container package over virtual machines. The [CNCF's Interactive Serverless Landscape](https://landscape.cncf.io/serverless?zoom=150) is a guide to open source projects, tools, frameworks, and public cloud platforms to enable DevOps teams to handle serverless applications.
