---
layout: post
title: Microservices reference architecture
date: 2019-07-17 00:00:00 +0300
description: Take a cloud-native approach to building mobile and web applications with a microservices architecture. # Add post description (optional)
img: microservice-reference-architecture.png # Add image post (optional)
tags: [Microservice, architecture] # add tag
---

Microservices for fast time to market and improved app quality
Take a cloud-native approach to building mobile and web applications with a microservices architecture.

Microservices is an application architectural style in which an application is composed of many discrete, network-connected components called microservices:
Large monolithic applications are broken into small services.
A single network-accessible service is the smallest deployable unit for a microservices application.
Each service runs in its own process. This rule, sometimes stated as "one service per container," might be a container or any other lightweight deployment mechanism, such as a Cloud Foundry runtime.

### Microservices reference architecture


In a microservices application architectural style, an application is composed of many discrete, network-connected components, termed microservices. The microservices architectural style is an evolution of the SOA (Services Oriented Architecture) architectural style. Applications built using SOA services tend to become focused on technical integration issues, and the level of the implemented services are often fine-grained technical APIs. In contrast, the microservices approach implements clear business capabilities through larger-grained business APIs.


The biggest difference between the two approaches is how they are deployed. For many years, applications have been packaged in a monolithic fashion – that is a team of developers constructed one large application that did everything required for a business need. Once built, that application was then deployed multiple times across a farm of application servers. In contrast, with the microservices architectural style, developers independently build and package several smaller applications that each implement only parts of the whole application.

### Functional requirements


Building microservices through APIs behind mobile and web applications.

Providing implementation choices for microservices such as Java, Node JS, Swift, and others.

Exposing microservices to front ends using API Connect.

Invoking APIs from native mobile clients built in iOS or Android and from web clients that use technologies like AngularJS or ReactJS.

Deploying microservices using different cloud workload patterns such as Docker, Cloud Foundry, and IBM Cloud Functions, which is based on Apache OpenWhisk.

Using microservices frameworks, such as Amalgam8 or Netflix OSS, to implement well known microservice patterns like routing, circuit breaker, and auto scaling.

Creating resilient microservices through the use of clustering, auto scaling, failover, circuit breaker, bulk head, and disaster recovery.

Using key services for front-end applications such as mobile analytics, push notifications, content management, and others.

Providing guidance for operating, monitoring, and managing microservice-based applications.

Building out end-to-end DevOps by providing detailed guidance on how to build continuous integration/continuous delivery pipelines for microservices and front ends.

Using Garage Method for Cloud in the context of microservices, such as test driven development.