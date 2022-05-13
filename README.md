# Introduction

[![GitHub stars](https://img.shields.io/github/stars/airbytehq/airbyte?style=social&label=Star&maxAge=2592000)](https://GitHub.com/airbytehq/airbyte/stargazers/) [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/airbytehq/airbyte/Airbyte%20CI)](https://github.com/airbytehq/airbyte/actions/workflows/gradle.yml) [![License](https://img.shields.io/static/v1?label=license&message=MIT&color=brightgreen)](https://github.com/airbytehq/airbyte/tree/a9b1c6c0420550ad5069aca66c295223e0d05e27/LICENSE/README.md) [![License](https://img.shields.io/static/v1?label=license&message=ELv2&color=brightgreen)](https://github.com/airbytehq/airbyte/tree/a9b1c6c0420550ad5069aca66c295223e0d05e27/LICENSE/README.md)


**Data integration made simple, secure and extensible.**
The new open-source standard to sync data from applications, APIs & databases to warehouses, lakes & other destinations.

Airbyte is on a mission to make data integration pipelines a commodity.

* **Maintenance-free connectors you can use in minutes**. Just authenticate your sources and warehouse, and get connectors that adapt to schema and API changes for you.
* **Building new connectors made trivial.** We make it very easy to add new connectors that you need, using the language of your choice, by offering scheduling and orchestration. 
* Designed to **cover the long tail of connectors and needs**. Benefit from the community's battle-tested connectors and adapt them to your specific needs.
* **Your data stays in your cloud**. Have full control over your data, and the costs of your data transfers. 
* **No more security compliance process** to go through as Airbyte is self-hosted. 
* **No more pricing indexed on volume**, as cloud-based solutions offer. 

Here's a list of our [connectors with their health status](integrations/README.md).

## Quick Start

```bash
git clone https://github.com/airbytehq/airbyte.git
cd airbyte
docker-compose up
```

Now visit [http://localhost:8000](http://localhost:8000)

Here is a [step-by-step guide](https://github.com/airbytehq/airbyte/tree/e378d40236b6a34e1c1cb481c8952735ec687d88/docs/quickstart/getting-started.md) showing you how to load data from an API into a file, all on your computer.

## Overview

* **Built for extensibility**: Adapt an existing connector to your needs or build a new one with ease.
* **Optional normalized schemas**: Entirely customizable, start with raw data or from some suggestion of normalized data.
* **Full-grade scheduler**: Automate your replications with the frequency you need.
* **Real-time monitoring**: We log all errors in full detail to help you understand.
* **Incremental updates**: Automated replications are based on incremental updates to reduce your data transfer costs.
* **Manual full refresh**: Sometimes, you need to re-sync all your data to start again.
* **Debugging autonomy**: Modify and debug pipelines as you see fit, without waiting.

[See more on our website.](https://airbyte.io/features/)


## Workshops

- [**Web Application**](https://webapp.serverlessworkshops.io) - This workshop shows you how to build a dynamic, serverless web application. You'll learn how to host static web resources with Amazon S3, how to use Amazon Cognito to manage users and authentication, and how to build a RESTful API for backend processing using Amazon API Gateway, AWS Lambda and Amazon DynamoDB.

- [**Auth**](https://auth.serverlessworkshops.io) - This workshop shows you how to build in security at multiple layers of your application, starting with sign-up and sign-in functionality for your application, how to secure serverless microservices, and how to leverage AWS's identity and access management (IAM) to provide fine-grained access control to your application's users. You'll learn how AWS Amplify integrates with Amazon Cognito, Amazon API Gateway, AWS Lambda, and IAM to provide an integrated authentication and authorization experience.

- [**Data Pipeline**](010-xdataiq/README.md) - This workshop demonstrates how to collect, store, and process data with a serverless application. In this workshop you'll learn how to build real-time streaming applications using Amazon Kinesis Data Streams and Amazon Kinesis Data Analytics, how to archive data streams using Amazon Kinesis Data Firehose and Amazon S3, and how to run ad-hoc queries on those files using Amazon Athena.

- [**DevOps**](https://cicd.serverlessworkshops.io/) - In this workshop, you will learn how to start a new Serverless application from scratch using the [Serverless Application Model (SAM)](https://github.com/awslabs/serverless-application-model) and how to fully automate builds and deployments by building a continous delivery pipeline using AWS CodeCommit, AWS CodeBuild and AWS CodePipeline. You will also learn how to test a Serverless application locally using the SAM CLI.

- [**Image Processing**](ImageProcessing) - This module shows you how to build a serverless image processing application using workflow orchestration in the backend. You'll learn the basics of using AWS Step Functions to orchestrate multiple AWS Lambda functions while leveraging the deep learning-based facial recognition features of Amazon Rekogntion.

- [**Multi Region**](MultiRegion) - This workshop shows you how to build a serverless ticketing system that is replicated across two regions and provides automatic failover in the event of a disaster. You will learn the basics of deploying AWS Lambda functions, exposing them via API Gateway, and configuring replication using Route53 and DynamoDB streams.

- [**Security**](https://github.com/aws-samples/aws-serverless-security-workshop) - This workshop shows you techniques to secure a serverless application built with AWS Lambda, Amazon API Gateway and RDS Aurora. We will cover AWS services and features you can leverage to improve the security of a serverless applications in 5 domains: identity & access management, infrastructure, data, code, and logging & monitoring.

- [**Machine Learning**](MachineLearning) - This workshop shows you how to collect, process, and join disparate data sources using AWS Lambda and Amazon Athena. This data can be used to train a machine learning model using Amazon SageMaker. With the trained model hosted on Amazon S3, you will build a serverless API using Amazon API Gateway and AWS Lambda to predict the probability that a unicorn will request service after completing a ride.

- [**Decoupled Microservices**](https://async-messaging.workshop.aws/) - This workshop demonstrates the use of asynchronous messaging patterns to build micro-services based architecture. It applies the well known enterprise integration patterns using AWS services like SQS and SNS to implement various use cases for wild rydes business. All the labs are self contained and users can choose to go on their own adventure based on their requirements.

- [**Document Processing**](https://document-processing.serverlessworkshops.io/) - This workshop demonstrates the use of AWS Lambda and Amazon Textract to extract text and data from large scale documents. It shows both asynchronous and synchronous architectural patterns to build an efficient document processing engine.

- [**Go Serverless**](https://golang.serverlessworkshops.io/) - In this workshop, you will learn by using Go and the AWS Serverless Application Model (SAM), how to create a simple web service using AWS Lambda functions. It will also cover testing and debugging your web service locally with SAM monitoring and also troubleshooting your web service with distributed tracing using AWS X-Ray.

- [**Application Catalog**](https://application-catalog.serverlessworkshops.io/) - In this workshop, we will explore some of the ways you can implement a CI/CD pipeline on AWS for Serverless workloads in a standardized way across an entire organization, allowing Software Engineers to develop and test Serverless workloads as they would in a more traditional environment while DevOps teams can focus on building one single pipeline that satisfies multiple environments and can be distributed as a “product” across multiple development teams.

- [**Event Driven Architecture**](https://event-driven-architecture.workshop.aws/) - In this workshop we’ll cover the basics of event-driven design, using examples that involve Amazon EventBridge, Amazon SNS, Amazon SQS, AWS Lambda and more. You will learn how to choose the right AWS service for the job, as well as how to optimize for both cost and performance. Through hands on practice, this workshop will give you the skills bring event-driven design patterns into your own applications.


## Contributing

We love contributions to xDataIQ, big or small.

Please refer to the [Contributing Guide](open-innovation/README.md) and [Contributing FAQ](open-innovation/FAQ.md) for details.


If you have any questions, please open a draft PR or visit our [slack channel](https://slack.xdataiq.com/) where the core team can help answer your questions.

**Note that you are able to create connectors using the language you want, as Airbyte connections run as Docker containers.**

**Also, we will never ask you to maintain your connector. The goal is that the Airbyte team and the community helps maintain it, let's call it crowdsourced maintenance!**

## Community support

For general help using Airbyte, please refer to the official Airbyte documentation. For additional help, you can use one of these channels to ask a question:

* [Slack](https://slack.airbyte.io) \(For live discussion with the Community and Airbyte team\)
* [Forum](https://discuss.airbyte.io/) \(For deeper converstaions about features, connectors, or problems\)
* [GitHub](https://github.com/airbytehq/airbyte) \(Bug reports, Contributions\)
* [Twitter](https://twitter.com/airbytehq) \(Get the news fast\)
* [Weekly office hours](https://airbyte.io/weekly-office-hours/) \(Live informal 30-minute video call sessions with the Airbyte team\)

## Roadmap

Check out our [Roadmap](https://app.harvestr.io/roadmap/view/pQU6gdCyc/airbyte-roadmap) to get informed on what we are currently working on, and what we have in mind for the next weeks, months and years.

## License

See the [LICENSE](project-overview/licenses/README.md) file for licensing information, and our [FAQ](project-overview/licenses/license-faq.md) for any questions you may have on that topic. 

