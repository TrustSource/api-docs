# API-Structure

To get a grip on APIv2 it is important to understand that TrustSource APIv2 comprises of different services. It is a basic REST API but also a comprehensive business API, allowing to initiate complex actions. You may manage a complete release through the API without the need for logging in. To not get lost, start thinking in the following categories:

1. **Core**

provides access to all elements within the application such as projects, modules and scans as well as the actions like approvals, releases and all sort of reporting.

2. **DeepScan** (or repository)

allows to execute the file based assessments and dig into the results of these.

3. **Vulnerabilities**

offers all sort of analysis and investigation information concerning vulnerabilities and weaknesses as well as CSAF2.0 related documents.

4. **ComponentBase**

grants access to our knowledge on compoenents. This is the aggregation of the knowledge that has been collected by our customers as well as our own clearing activity. Findings from DeepScan results are added to general index data, etc. 

5. **Compliance Information**

allows to publish your achievements towards 3rd parties. This especially comprises required documents for particular releases such as NoticeFiles, SOUP lists or CSAF VEX documents or company information like FOSS Liason. Here we also offer functionality to verify the originality of documents.

> [!IMPORTANT]
>
> **PLEASE NOTE:** The APIv2 has a file upload limit of 1MB. This has been a security decision to prevent overloading. However, we are aware that 1MB is not very much when it comes to complex projects or scans. If you require larger uploads, please contact our [Support](mailto:support@trustsource.io).

The following sections will give a short introduction into each block. To test the API, go to [TrustSource App](https://app.trustsource.io) - you may register for free using a git-account - and click the book icon in the upper right corner of the screen. There you will find a SWAGGER allowing you to play around and experience the API functions. 
