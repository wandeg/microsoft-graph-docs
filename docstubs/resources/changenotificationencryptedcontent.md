---
title: "changeNotificationEncryptedContent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# changeNotificationEncryptedContent resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|data|String||
|dataKey|String||
|dataSignature|String||
|encryptionCertificateId|String||
|encryptionCertificateThumbprint|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationEncryptedContent",
  "data": "String",
  "dataSignature": "String",
  "dataKey": "String",
  "encryptionCertificateId": "String",
  "encryptionCertificateThumbprint": "String"
}
```

