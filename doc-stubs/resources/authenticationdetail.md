---
title: "authenticationDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# authenticationDetail resource type

Namespace: microsoft.graph

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
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationDetail",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "succeeded": "Boolean",
  "authenticationStepResultDetail": "String",
  "authenticationStepRequirement": "String"
}
```

