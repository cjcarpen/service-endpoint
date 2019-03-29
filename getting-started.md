---

copyright:
  years: 2018, 2019
lastupdated: "2019-03-29"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}

# About

Consumption of cloud services continues to grow across all industries. As more and more customers get 
comfortable with using cloud based services for their production workloads an increased scrutiny on security is being 
required. For many of our most sensitive customers, accessing services in a secure manner is not only a sensible 
corporate policy but, in some cases, required by compliance regulations that govern these companies.
IBM has enhanced their connectivity options for customers who require isolated connectivity options for 
their workloads. 

IBM Cloud Service Endpoint allows customers to connect to IBM Cloud services over the IBM 
Cloud private network. 
Moving these workloads from IBM Cloud's public network offers two advantages to the client.
1. Services are no longer being served on an internet routable IP address. It is becoming increasingly common for
cloud consumers to want limited or no access to the public internet from any of their services. Now with 
Service Endpoint, service teams can create an interface over the private network for their service which customers can use to connect. Internet access is no longer a requirement for customers to connect to IBM Cloud services.

2. There is no billed or metered bandwidth charges on IBM Cloud's private network. In the past, customers would be billed for egress bandwidth when talking to an IBM Cloud service. 

With IBM Cloud Service Endpoint, the solution becomes more appealing from a security and a consumption standpoint.

The following figure shows how traffic is routed through IBM Cloud's private network when accessing cloud services through Service Endpoints:


![IBM Cloud Service Endpoint](images/CSE.png)
