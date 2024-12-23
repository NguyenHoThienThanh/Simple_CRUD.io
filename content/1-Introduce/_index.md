---
title : "Introduction"

weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

## Introduction

In today's cloud-native world, serverless architectures are gaining significant traction due to their scalability, cost-efficiency, and ease of maintenance. This project demonstrates how to build a simple CRUD (Create, Read, Update, Delete) API using **AWS Lambda**, **API Gateway**, and **MongoDB**. These technologies provide powerful tools for developing scalable and cost-effective web applications with minimal operational overhead.

### What is AWS Lambda?

AWS Lambda is a serverless compute service that automatically manages the compute resources required to run your code in response to events. With Lambda, you don't need to provision or manage servers, making it ideal for building microservices and APIs in a highly scalable environment.

### What is API Gateway?

AWS API Gateway is a fully managed service that enables developers to create and publish RESTful APIs for their backend services. It acts as a gateway for HTTP requests, connecting clients to AWS Lambda functions, enabling secure, highly scalable API management.

### Why MongoDB?

MongoDB is a NoSQL database that offers flexibility and scalability. It’s a perfect choice for applications that require rapid development and high scalability. In this project, MongoDB will be used to store the data handled by the CRUD API, ensuring the application can manage large volumes of data and traffic efficiently.

### Objective

The goal of this project is to guide you through the process of building a simple CRUD API that:

1. Allows clients to interact with data stored in a MongoDB database.
2. Utilizes AWS Lambda functions for each CRUD operation, ensuring the API is serverless and scalable.
3. Leverages AWS API Gateway to route HTTP requests and securely interact with the Lambda functions.

By the end of this project, you will have a fully functioning serverless API capable of handling various data management tasks, without the need for managing infrastructure or scaling concerns.