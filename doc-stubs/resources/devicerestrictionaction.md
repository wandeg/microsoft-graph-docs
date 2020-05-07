---
title: "deviceRestrictionAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceRestrictionAction resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [dlpActionInfo](../resources/dlpactioninfo.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|dlpAction|**TODO: Add Description** Inherited from [dlpActionInfo](../resources/dlpactioninfo.md). Possible values are: `notifyUser`, `blockAccess`, `deviceRestriction`.|
|message|String|**TODO: Add Description**|
|restrictionAction|restrictionAction|**TODO: Add Description**. Possible values are: `warn`, `audit`, `block`.|
|triggers|restrictionTrigger collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceRestrictionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceRestrictionAction",
  "action": "String",
  "restrictionAction": "String",
  "triggers": [
    "String"
  ],
  "message": "String"
}
```

