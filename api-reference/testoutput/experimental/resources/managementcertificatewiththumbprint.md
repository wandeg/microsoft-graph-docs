---
title: "managementCertificateWithThumbprint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managementCertificateWithThumbprint resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificate|String|The Base 64 encoded management certificate|
|thumbprint|String|The thumbprint of the management certificate|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```

