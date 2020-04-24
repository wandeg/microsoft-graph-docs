---
title: "changeNotificationCollection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# changeNotificationCollection resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|validationTokens|String collection|**TODO: Add Description**|
|value|[changeNotification](../resources/changenotification.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationCollection",
  "validationTokens": [
    "String"
  ],
  "value": [
    {
      "@odata.type": "microsoft.graph.changeNotification",
      "subscriptionId": "Guid",
      "subscriptionExpirationDateTime": "String (timestamp)",
      "clientState": "String",
      "changeType": "String",
      "resource": "String",
      "tenantId": "Guid",
      "encryptedContent": {
        "@odata.type": "microsoft.graph.changeNotificationEncryptedContent",
        "data": "String",
        "dataSignature": "String",
        "dataKey": "String",
        "encryptionCertificateId": "String",
        "encryptionCertificateThumbprint": "String"
      },
      "lifecycleEvent": "String",
      "resourceData": {
        "@odata.type": "microsoft.graph.resourceData"
      }
    }
  ]
}
```

