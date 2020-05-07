---
title: "onPremisesPublishing resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onPremisesPublishing resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateUrl|String|**TODO: Add Description**|
|applicationServerTimeout|String|**TODO: Add Description**|
|applicationType|String|**TODO: Add Description**|
|externalAuthenticationType|externalAuthenticationType|**TODO: Add Description**. Possible values are: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|**TODO: Add Description**|
|internalUrl|String|**TODO: Add Description**|
|isHttpOnlyCookieEnabled|Boolean|**TODO: Add Description**|
|isOnPremPublishingEnabled|Boolean|**TODO: Add Description**|
|isPersistentCookieEnabled|Boolean|**TODO: Add Description**|
|isSecureCookieEnabled|Boolean|**TODO: Add Description**|
|isTranslateHostHeaderEnabled|Boolean|**TODO: Add Description**|
|isTranslateLinksInBodyEnabled|Boolean|**TODO: Add Description**|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](../resources/onpremisespublishingsinglesignon.md)|**TODO: Add Description**|
|useAlternateUrlForTranslationAndRedirect|Boolean|**TODO: Add Description**|
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](../resources/verifiedcustomdomaincertificatesmetadata.md)|**TODO: Add Description**|
|verifiedCustomDomainKeyCredential|[keyCredential](../resources/keycredential.md)|**TODO: Add Description**|
|verifiedCustomDomainPasswordCredential|[passwordCredential](../resources/passwordcredential.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesPublishing",
  "externalUrl": "String",
  "internalUrl": "String",
  "externalAuthenticationType": "String",
  "isTranslateHostHeaderEnabled": "Boolean",
  "isTranslateLinksInBodyEnabled": "Boolean",
  "isOnPremPublishingEnabled": "Boolean",
  "applicationServerTimeout": "String",
  "verifiedCustomDomainKeyCredential": {
    "@odata.type": "microsoft.graph.keyCredential"
  },
  "verifiedCustomDomainPasswordCredential": {
    "@odata.type": "microsoft.graph.passwordCredential"
  },
  "verifiedCustomDomainCertificatesMetadata": {
    "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata"
  },
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn"
  },
  "applicationType": "String",
  "isHttpOnlyCookieEnabled": "Boolean",
  "isSecureCookieEnabled": "Boolean",
  "isPersistentCookieEnabled": "Boolean",
  "alternateUrl": "String",
  "useAlternateUrlForTranslationAndRedirect": "Boolean"
}
```

