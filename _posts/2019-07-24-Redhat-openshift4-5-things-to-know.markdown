---
layout: post
title: Red Hat OpenShift 4 Kubernetes Platform--5 Things To Know
date: 2019-07-24 00:00:00 +0300
description: In terms of Red Hat’s emerging products, OpenShift is out in the lead, because it's capitalizing on key trends including hybrid cloud, Kubernetes and containers, and DevOps and cloud-native application development, according to Joe Fernandes, Red Hat’s vice president of products for cloud platforms.
img: red-hat-openshift-4.jpg # Add image post (optional)
tags: [OpenShift4, kubernetes,Redhat] # add tag
---

Red Hat unveiled its new enterprise-grade OpenShift 4, its first new major iteration of the Kubernetes platform since it was rebuilt around the open-source container orchestration system four years ago.

OpenShift 4, unveiled at the Red Hat Summit in Boston and expected to be available in the next month, is designed with full-stack automation for a cloud-like experience, allowing developers to run container-based software applications in hybrid cloud environments.

OpenShift 4 is designed to deliver a cloud-like experience across the hybrid cloud by driving automated updates across Kubernetes deployments everywhere. OpenShift 4 brings a new ray of light in the container space due to the numerous advancements done on the platform. (source: www.redhat.com, 2019). The following are some of the amazing stuff done on the platform:

![Openshift4](/assets/img/redhat-openshift-4-new-features.png)

“We put more focus on how people manage the platform and how they manage apps that run on the platform,” said Joe Fernandes, Red Hat’s vice president of products for cloud platforms. “What we're seeing is people are deploying more and more different types of applications, more complex applications, for things like databases or messaging solutions or (artificial intelligence) and machine learning. So as the universe of application workloads expands, people need better tools to manage them, because those apps aren't just simple, cloud-native apps.”

In terms of Red Hat’s emerging products, OpenShift is out in the lead, because it's capitalizing on key trends including hybrid cloud, Kubernetes and containers, and DevOps and cloud-native application development, according to Fernandes.

“These things are in high demand, and OpenShift kind of brings that together,” he said.

Red Hat said it’s almost doubled the number of OpenShift customers to include more than 1,000 enterprises that use it for application development and delivery, including Banco Santander, BMW, BP, Cathay Pacific, Deutsche Bank, Emirates NBD, ExxonMobil, General Electric, Kohl’s and Volkswagen.

What follows are some of the key features of OpenShift 4.

### 5. OperatorHub Framework

New to OpenShift 4 is single-step installation for Kubernetes applications and services, and automated, over-the-air updates and performance tuning with Kubernetes Operators.
![OperatorHub](https://www.redhat.com/cms/managed-files/styles/wysiwyg_full_width/s3/880_440_v11-categories@2x_0.png?itok=1BEJ3StF)
Red Hat last year launched a new upstream project called the Operator Framework, an open-source toolkit designed to manage Kubernetes-native applications, known as Operators, in a more automated and scalable way.

“Operators basically allow you to extend Kubernetes with management capabilities that are specific to the different types of services that you may want to run,” Fernandes said. “We took this Operator concept and said we can apply this both to work with our partners for better managing the stuff that they want to run on top of OpenShift, and then we can use this ourselves to better manage the platform and make it more automated.”

Red Hat introduced Red Hat OpenShift Operator Certification to validate the work of its independent software vendor partners.

“OpenShift 4 is the first time we fully support Operators, and then the certification program kind of layers on top of that feature,” Fernandes said. “The certification is how do we enable partners to take advantage of this feature and jointly certify and support the capabilities that they built with it. The goal of certification is to basically say, even though anybody can take advantage of this technology, we've worked together with select partners to make sure that we got it right and that we're basically addressing the needs of our joint customers.”

### 4. OpenShift is now a Trusted Enterprise Kubernetes


Red Hat OpenShift Container Platform is certified, conformant Kubernetes, as validated by the Cloud Native Computing Foundation (CNCF). At the moment, it is the only enterprise Kubernetes offering built on the backbone of the world’s leading enterprise Linux platform. Moreover it is backed by the open source expertise, compatible ecosystem, and leadership of Red Hat (source: www.redhat.com, 2019).


### 3. Kubernetes at the Core with Full Stack Automation

OpenShift 4 is Kubernetes at its core and in this release they have completely re-architected how to install, upgrade and manage the platform. There is advanced day 2 management and automation to the application services that run on the platform. Some of the Automation details include (www.redhat.com, 2019):

- Self-managing platform for hybrid cloud to provide a cloud-like experience via automatic software updates and lifecycle management. This happens across the hybrid cloud, powered by the trusted foundation of Red Hat Enterprise Linux and Red Hat Enterprise Linux CoreOS.

- Adaptability and heterogeneous support, available in coming months across major public cloud vendors. Such as Alibaba, Amazon Web Services (AWS), Google Cloud, IBM Cloud, Microsoft Azure. This ancludes private cloud technologies like OpenStack, virtualization platforms and bare-metal servers.

- Get started with enterprise Kubernetes easily using streamlined full stack installation with an automated process.

- Simplified application deployments and lifecycle management with Kubernetes Operators.


### 2. OpenShift Service Mesh

Red Hat is bringing support for Istio in OpenShift 4 through what's called the OpenShift service mesh, which is designed for increased resiliency and performance of distributed applications.

![Istio Architecture](https://istio.io/docs/concepts/what-is-istio/arch.svg)

Istio is an open-source project for microservice developers to help them build and debug microservices-based applications, and Red Hat has been heavily involved in the project.

### 1. Knative Framework

The Knative framework, in developer preview, is a new developer-friendly serverless framework for building, serving and running event-driven applications.

Knative includes scale-to-zero, autoscaling, in-cluster builds and eventing frameworks for developing cloud-native applications on Kubernetes. It allows developers to focus on writing code by hiding complex parts of building, deploying and managing their applications, according to Red Hat.

“Serverless is a key component of function-as-a-service offerings like AWS Lambda or Azure Functions or Google Cloud Functions,” Fernandes said. “This is sort of a new style of programming, basically using functions to add functionality to your applications versus having stuff that runs all the time. We've seen developers really begin to adopt this technology. But the problem is, it's typically available in a specific cloud. We wanted to create something that could work across multiple clouds and also work in the data center.”

“It's in developer preview, so it's not fully supported yet, but it's something that we've been building for the past year, and it’ll be releasing in the next six months or so on top of OpenShift 4,” Fernandes said. “We want to get it into more customers hands and let them play with it and tell us what they think.”


## Kubernetes at the Core with Full Stack Automation

OpenShift 4 is Kubernetes at its core and in this release we have completely re-architected how we install, upgrade and manage the platform, while also bringing advanced day 2 management and automation to the application services that run on the platform. These advancements are based on many new innovations in the Kubernetes ecosystem, none bigger than Kubernetes Operators.

Operators automate life cycle management of containerized applications with Kubernetes. With Operators, administrators can extend the Kubernetes API to codify operational knowledge and workflows for managing complex applications right into those services, so they run seamlessly on Kubernetes. For OpenShift customers and ISV partners, this allows them to bring the same level of management and automation found in public cloud services to their own services, while providing a consistent operating model for running these services across the hybrid cloud.

Since OpenShift itself is a fully containerized platform consisting of many different components, we also take advantage of Operators for driving the installation and upgrades of OpenShift and all of its services. This includes Kubernetes core services, along with Prometheus, Grafana, Elasticsearch, software defined networking, storage, registry and other components that make up the OpenShift Kubernetes platform. OpenShift 4 is an Operator-driven platform that delivers full-stack automation from top to bottom. From Kubernetes, to the core services that support the OpenShift cluster, to the application services deployed by end users; everything is managed throughout its lifecycle with Operators.