---
title: "authenticationRequirementPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authenticationRequirementPolicy resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|detail|String||
|requirementProvider|Enumeration| Possible values are: `MFA`, `CA`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.authenticationRequirementPolicy"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.authenticationRequirementPolicy",
  "requirementProvider": "String",
  "detail": "String"
}
```

