---
title: "authenticationRequirementPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# authenticationRequirementPolicy resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detail|String|**TODO: Add Description**|
|requirementProvider|requirementProvider|**TODO: Add Description**. Possible values are: `MFA`, `CA`, `unknownFutureValue`.|

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

