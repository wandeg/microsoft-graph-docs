---
title: "changeNotification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# changeNotification resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeType|Enumeration| Possible values are: `created`, `updated`, `deleted`.|
|clientState|String||
|encryptedContent|[changeNotificationEncryptedContent](../resources/changenotificationencryptedcontent.md)||
|lifecycleEvent|Enumeration| Possible values are: `missed`, `subscriptionRemoved`, `reauthorizationRequired`.|
|resource|String||
|resourceData|[resourceData](../resources/resourcedata.md)||
|subscriptionExpirationDateTime|DateTimeOffset||
|subscriptionId|Guid||
|tenantId|Guid||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotification",
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
```

