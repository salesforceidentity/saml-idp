saml-idp
=================

## March 2023 Update

 Salesforce1 Platform has a built-in SAML Identity Provider. This project isn't needed for production deployments. Learn more here: [Enable Salesforce as a SAML Identity Provider](https://help.salesforce.com/s/articleView?id=sf.identity_provider_enable.htm&type=5)

## What is this?
A sample SAML IdP implementation in Apex.  It is SP-init only and supports HTTP Redirect binding for Requests, and HTTP POST for Responses.  Tested against Google.  

## To get started:

1. Create an Object called SAML_Service_Provider__c with ACS_URL__c	URL(255), CertificateName__c Text(255), Entity_ID__c Text(255) (Unique Case Insensitive), and Issuer__c Text(255)
2. Upload the static resource as public and all it js_inflate
3. Create the code from the Apex, and Pages directory
4. Adjust permissions on your profiles to allow the proper users to be able to excute the management and SPInit endpoints
5. Generate a self-signed cert in Key and Certificates ( if you don't have one already )
6. Go to /apex/SAMLManagement and configure a Service Provider

Now, you can have your Service Providers SP-init against /apex/SAMLSPInit.   


