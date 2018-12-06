---

copyright:
  years: 2017, 2018
lastupdated: "2018-07-25"

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
comfortable with using cloud based services for their production workload an increased scrutiny on security is being 
required. For many of our most sensitive customers, accessing services in a secure manner is not only a sensible 
corporate policy but, in some cases, required by the many compliance regulations that govern these companies.
IBM has enhanced their connectivity options for customers who require isolated connectivity options for 
their workloads. 

IBM Cloud Service Endpoint allows customers to connect to IBM service through the internal IBM 
Cloud network. 
Moving these workloads from IBM’s public cloud network offers two advantages to the client.
1. Services are no longer being served on an internet routable IP address. It is becoming increasingly more common for
cloud consumers to want limited or no access to the public internet from any of their services. Now with 
Service Endpoints, service teams can create an internal interface for their service and customers can connect using their internal network interfaces. Internet access is no longer a requirement for customers to connect to IBM services.

2. There is no billed or metered bandwidth charges on IBM’s internal network. In the past, customers would be billed for egress bandwidth when talking to an IBM Cloud service. 

With IBM’s Service Endpoint, the solution becomes more appealing from a financial and a consumption standpoint.

The following figure shows how traffic is routed through IBM Cloud's internal network when accessing cloud services:


![IBM Cloud Service Endpoint](images/CSE.png)
