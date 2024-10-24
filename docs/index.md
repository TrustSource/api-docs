# TrustSource APIv2

This **API documentation** addresses the recently released v2 of the TrustSource platform API.  

Feel free to reach out anytime, to clarify questions through mail under ```support @ trustsource.io``` or contact - in case you are a paying subscriber - your account representative.



## Introduction
TrustSource helps in providing Security and Compliance along the Software Supply Chain. Since large parts of these tasks, if not already, will be automated, a capable API is an important success factor to successfully securing the Software Supply Chain. At TrustSource we focus on leveraging our customer's efficiency through optimal integration. We provide a collection of servcies and tools to simplify operations, to keep their back free from the hazzle and insufficiencies comprising the tooling landscape around open source compliance and security. TrustSource has been assembled over years to support a fully managed solution coping with all aspects of Software Supply Chain Security. 

However, if you feel like something is missing or should be integrated better, please do not hesitate to participate or reach out to us, so that we may explore on how to bridge the gap.

## Scope
This document addresses the use of TrustSource API in general and describes underlying concepts and ideas. It will address the most recent version, which currently is v2. However, the deltas to v1 will be outlined where new functionality appears. Te learn more how to migrate, see the section on **Migrating APIv1 to APIv2**.

## Table of Contents

This documentation is structured into six sections with differnt focus:

1. This Introduction, which guides you through the idea and reading hints
2. [Key Management](/api-docs/keymgmt) - Introduction to API keys and how to manage them 
3. [Roles](/roles) - This section gives an overview of the TrsutSource roles you may use to scope your keys. 
4. [API Structure](/api-docs/structure) - Here you get insights on our data management and will learn what you may do to ensure integrity from your side
5. [API Analytics](/api-docs/analytics) - Gives you ideas on how to keep control over API usage
6. [Use Cases](/api-docs/usecases) - Collection of use cases describing how to tackle specific obstacles that may appear when securing your Software Supply Chain 



> [!IMPORTANT]
>
> **PLEASE NOTE:** APIv1 has been shut down ***September 30th, 2024***. Requests will only return 410.



## How to read the document

If you are a new user and have endless time, we suggest to read everyting from beginning to start. But most likely you already denied the second condition and thus are seeking a way to reduce the time to achieve your goal. In this case follow one of the role-specific paths outlined here:

- **System Administrator / Operations**

You should at least understand the [Key Management](/api-docs/keymgmt). If you plan to distribute expenses across your users, [API Analytics](/api-docs/analytics) will also be of value to you.

- **Security Architect**

We suggest to gain an idea on the api [key scopes](/api-docs/keymgmt) and then dive into the use cases. 

- **Project or Product Manager**

Be sure to get an idea of understand the [Key Management](/api-docs/keymgmt).

- **Compliance Manager**

Have a look into the  [API Structure](/api-docs/structure) to gain an understanding of the options you will gain through the compliance API.

- **CI/CD Operator / Developer**

You may focus on the introductions of chapters 3, 4, 5 and 6. The details you may add upon demand.



## Migrating APIv1 to APIv2

The APIv2 has been implemented during December 2023. Meanwhile (Oct/24) v1 is not even supported anymore. However, some of our older scanning tools may still want to connect to https://app.trustsource.io/api/v1/... To switch API, you should upgrade to the öatest version or find the config file, where to set the target URL. See the corresponding repo for details. To find the repo use [TrustSource Repo Overview](https://github.com/trustsource) as starting point for your search.

To migrate, you will just need to point your requests to the URL [https://api.trustsource.io/v2/](https://api.trustsource.io/v2/) instead the the former https://app.trustsource.io/api/v1/ base url. ***All functionality is fully backward compatible.*** To learn about new functionality and experiment/play with the functions, visit the API documentation inside [TrustSource Service](https://app.trustsource.io/apidoc-latest).



## Further Sources of Knowledge

You should be aware of the different sources you may tap to learn about TrustSource:

- Tools: TrustSource provides a huge collection of services and tools. Most of our tools are provided as opensource and can be found on [Github](!https://github.com/trustsource)
- System Monitoring: at the bottom of each screen you will find a link to our public [System Monitoring](!https://status.trustsource.io)
- System Management Notifications: in the above linked page you will be able to subscribe to a newsletter, where will announce changes and system updates. 
- Knowledge Base: at the top right of the application there is a link to our online [Knowledge base](!https://support.trustsource.io)
- FAQ: the Knowledgebase is available to everyone and contains information on compliance, establishing Compliance processes, setting up an OSPO, integrating different programming languages / CI/CD flows with TrustSource, how to handle use cases within TrustSource, etc.
- If you are subscribed to TrustSource you also are eligible to may write an email to our support team at [support@trustsource.io](mailto:support@trustsource.io)
- Direct contact: You will find our contact details, at our website under [www.trustsource.io/contact](!https://www.trustsource.io/contact)


## License

This documentation is provided under CC-BY-SA-4.0. You may clone or fork this repository and create you own documentation based on these documents. But please make sure to remove all references to TrustSource and EACG except an attribution notice. **EACG** as well as **TrustSource** and the corresponding logos are protected Trademarks and should not be used without a written approval by any third party.

This documentation may change. We will notify changes through the systems management notification mailing list.

