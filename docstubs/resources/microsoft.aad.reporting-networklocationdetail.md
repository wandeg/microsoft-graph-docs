---
title: "networkLocationDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# networkLocationDetail resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|networkNames|String collection||
|networkType|Enumeration| Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.networkLocationDetail"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.networkLocationDetail",
  "networkType": "String",
  "networkNames": [
    "String"
  ]
}
```

