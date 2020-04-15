---
title: "authenticationDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authenticationDetail resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationMethod|String||
|authenticationMethodDetail|String||
|authenticationStepDateTime|DateTimeOffset||
|authenticationStepRequirement|String||
|authenticationStepResultDetail|String||
|succeeded|Boolean||

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

