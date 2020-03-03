---
title: "notifyUserAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# notifyUserAction resource type




Inherits from [dlpActionInfo](../resources/dlpActionInfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Inherited from [dlpActionInfo](../resources/dlpActionInfo.md). Possible values are: `notifyUser`, `blockAccess`, `deviceRestriction`.|
|actionLastModifiedDateTime|DateTimeOffset||
|emailText|String||
|overrideOption|Enumeration|. Possible values are: `notAllowed`, `allowFalsePositiveOverride`, `allowWithJustification`, `allowWithoutJustification`.|
|policyTip|String||
|recipients|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.notifyUserAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notifyUserAction",
  "action": "String",
  "recipients": [
    "String"
  ],
  "actionLastModifiedDateTime": "String (timestamp)",
  "overrideOption": "String",
  "emailText": "String",
  "policyTip": "String"
}
```

