---
title: "deviceRestrictionAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceRestrictionAction resource type


Namespace: microsoft.graph




Inherits from [dlpActionInfo](../resources/dlpactioninfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Inherited from [dlpActionInfo](../resources/dlpactioninfo.md). Possible values are: `notifyUser`, `blockAccess`, `deviceRestriction`.|
|message|String||
|restrictionAction|Enumeration| Possible values are: `warn`, `audit`, `block`.|
|triggers|Enumeration collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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

