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

![](https://github.com/DrVicki/back-end-development/blob/main/cncf-serverless-landscape.png)
(CNCF, Apache License 2.0)

Developers can write code and deploy it quickly to various serverless environments. The serverless application responds to demand and automatically scales up and down as needed.

If you are wondering what programming language and runtime are best suited for serverless application development to integrate with the technologies in the figure above; there's not just one answer to this question. 
- Let's discuss the application runtime most popular for developing business applications in enterprise production environments: Java.

According to [Developer Economics](https://developereconomics.com/), as of Q3 2020, more than 8 million enterprise developers use Java to achieve their business requirements. Yet, according to a [2020 NewRelic](https://newrelic.com/resources/ebooks/serverless-benchmark-report-aws-lambda-2020) survey, Java (at 6%) is clearly not the top choice for forward-thinking developers using a popular cloud service.

![](https://github.com/DrVicki/back-end-development/blob/main/newrelic_serverlessbenchmarkreport.png)
<br> Data from [NewRelic's Serverless Benchmark Report](https://newrelic.com/resources/ebooks/serverless-benchmark-report-aws-lambda-2020)

Resource usage, response times, and latency are critical in serverless development. 
- Serverless offerings from public cloud providers are typically metered on-demand, charged only when a serverless application is up, through an event-driven execution model. 
  - As a result; enterprises don't pay anything when a serverless application is idle or scaled down to zero.

## Java with containers

You may be wondering: "Why don't developers use the Java stack for serverless application development knowing existing business applications are most likely developed on Java technologies?"

Here is the truth: It's complicated to optimize Java applications in the new immutable infrastructure, also known as container platforms (e.g., Kubernetes).
