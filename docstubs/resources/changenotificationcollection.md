---
title: "changeNotificationCollection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# changeNotificationCollection resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|validationTokens|String collection||
|value|[changeNotification](../resources/changenotification.md) collection||

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
        "data": "binary",
        "dataSignature": "binary",
        "dataKey": "binary",
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

