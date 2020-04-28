---
title: "networkLocationDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# networkLocationDetail resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|networkNames|String collection|**TODO: Add Description**|
|networkType|networkType|**TODO: Add Description**. Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.|

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

