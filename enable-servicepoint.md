---

copyright:
  years: 2018
lastupdated: "2018-12-11"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}

# Getting Started

To get started with IBM Cloud Service Endpoint you need to make sure you have the following. 
1. An IBM Cloud Infrastructure Account 
2. Account must be enabled for Virtual Routing and Forwarding (VRF). Learn more about VRF on IBM Cloud [here](https://console.bluemix.net/docs/infrastructure/direct-link/vrf-on-ibm-cloud.html#overview-of-virtual-routing-and-forwarding-vrf-on-ibm-cloud). 
3. Account must be enabled for connectivity to Service Endpoints. 


## Enabling your account for using Service Endpoints using IBM Cloud CLI
{: #cs_cli_install_steps}


<br>
To install the CLIs:

1.  As a prerequisite for using Service Endpoints, install the [{{site.data.keyword.Bluemix_notm}} CLI](../cli/index.html#overview). The prefix for running commands by using the {{site.data.keyword.Bluemix_notm}} CLI is `ibmcloud`. Make sure the CLI version is 0.13. 

2.  Log in to the {{site.data.keyword.Bluemix_notm}} CLI. Enter your {{site.data.keyword.Bluemix_notm}} credentials when prompted.

    ```
    ibmcloud login
    ```
    {: pre}

    If you have a federated ID, use `ibmcloud login --sso` to log in to the {{site.data.keyword.Bluemix_notm}} CLI. Enter your user name and use the provided URL in your CLI output to retrieve your one-time passcode. You know you have a federated ID when the login fails without the `--sso` and succeeds with the `--sso` option.
    {: tip}

3.  Check if your account is already enabled for Service Endpoints.

    ```
    ibmcloud account show 
    ```
    {: pre}

    Example CLI output:

    ```
    Retrieving account Mark Anderson's Account of m.anderson@gmail.com...
    OK
                                 
     Account ID:                   d154dfbd0bc2edefthyufffc9b5ca318   
     Currently Targeted Account:   true   
     Linked Softlayer Account:     1008967   
     Service Endpoint Enabled:     false  
     ```
     {: screen}
            
    If 'Service Endpoint Enabled' is neither True or False, run the following command to initiate the IaaS configurations. 
    
     ```
    ibmcloud sl init
    ```
    {: pre}
    
    If Service Endpoint Enabled is True, your account is already enabled to acces Service Endpoints exposed by IBM Cloud Services on the cloud catalog. 

4.  If Service Endpoint Enabled is False, run the following command to enable it.

    ```
    ibmcloud account update --service-endpoint-enable true
    ```
    {: pre}
    
    This will prompt the user to open a support ticket with IBM Cloud to enable this account to use Service Endpoints. 
    Example CLI output:
    
    ```
    Service Endpoint is not available in linked Softlayer Account 1008967. 
    Enable VRF(Virtual Routing and Forwarding) first to proceed. 
    Learn more about VRF here - https://cloud.ibm.com/docs/infrastructure/direct-link/vrf-on-ibm-cloud.html.
    
    Do you want to open a ticket to enable it?[y/N]> y
    Ticket 70729615 was opened successfully. Follow the link https://control.softlayer.com/support/tickets/70729876 to check   the details and track the status of the ticket. You will be required to login to view this ticket.
    Account ID:    1008967
    Ticket:        Private Network Question - Enable Service Endpoint connectivity for my account 
    ```
    {: screen}
   
5. Once the account is enabled for Service Endpoints, one can start comsuming the Service Endpooints of IBM Cloud Services that have exposed this functionality. 

<br/>

In the very near future support case creation will be automated through the IBM Cloud Console. Additonal updates will be included here when these capabilities are available. 
