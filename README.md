# Experience Cloud - Adobe Exchange Partner API
Partner API specification that needs to be implemented by Experience Cloud Extension developers, who are consuming product APIs via Adobe I/O

## Introduction

### What is Adobe Exchange?
[Adobe Exchange](https://exchange.adobe.com) is a marketplace for all Adobe product extensions / plugins / apps / integrations.

### How do I list my extension on the Exchange?
You can join one of the partner programs found [here](https://www.adobe.com/partners.html) and start building apps for Creative / Experience / Document Cloud prodcuts. This documentation is specifically for partners enrolled in [Adobe Exchange Partner Program for Experience Cloud](https://partners.adobe.com/exchangeprogram/experiencecloud.html).

## What's the Partner API?

### Context
To create extensions for Experience Cloud products, like Adobe Analytics, Campaign, Target, you might be required to use [product APIs](https://www.adobe.io/apis.html) For eg. [Adobe Analytics API](https://www.adobe.io/apis/experiencecloud/analytics/docs.html).
To authenticate with the APIs, the [Adobe I/O Authentication](https://www.adobe.io/authentication/auth-methods.html#!AdobeDocs/adobeio-auth/master/AuthenticationOverview/AuthenticationGuide.md) mechanism needs to be followed.

### Problem
As a partner/developer, you would require your customer to create an I/O Integration on the Adobe I/O console, using your public key certificate (or their own - in which case they'll have to share it's private key with you); and share the integration client ID and secret with you.
This would allow you to access your customer's Analytics (or respective Adobe Experience Cloud product) data via API. But this is an offline manual process.

### Solution
Adobe Exchange will facilitate creation of this integration, public-private key pair and transfer the required credentials to the partner. To transfer, the partners need to register an API endpoint (at the time of creating an app listing) with Exchange where the credentials could be POSTed.
The detailed specification of that API is provided in this repo as a swagger.yaml . This is the Partner API.


The Partner API Endpoints are explained [here](https://adobeexchangeec.zendesk.com/hc/en-us/articles/360028551691-Adobe-Exchange-App-Manager-API-URLs).

The Partner API Swagger playground is [here](https://adobedocs.github.io/OAE_PartnerAPI/).


## Contributing
Contributions are welcome! Read the [Contributing Guide](CONTRIBUTING.md) for more information.

## Licensing
This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
