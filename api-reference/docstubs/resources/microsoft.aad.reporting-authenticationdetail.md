---
title: "authenticationDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# authenticationDetail resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationMethod|String|**TODO: Add Description**|
|authenticationMethodDetail|String|**TODO: Add Description**|
|authenticationStepDateTime|DateTimeOffset|**TODO: Add Description**|
|authenticationStepRequirement|String|**TODO: Add Description**|
|authenticationStepResultDetail|String|**TODO: Add Description**|
|succeeded|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.authenticationDetail"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.authenticationDetail",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "succeeded": true,
  "authenticationStepResultDetail": "String",
  "authenticationStepRequirement": "String"
}
```

