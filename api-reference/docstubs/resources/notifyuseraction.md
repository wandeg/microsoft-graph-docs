---
title: "notifyUserAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# notifyUserAction resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [dlpActionInfo](../resources/dlpactioninfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|dlpAction|**TODO: Add Description** Inherited from [dlpActionInfo](../resources/dlpactioninfo.md). Possible values are: `notifyUser`, `blockAccess`, `deviceRestriction`.|
|actionLastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|emailText|String|**TODO: Add Description**|
|overrideOption|overrideOption|**TODO: Add Description**. Possible values are: `notAllowed`, `allowFalsePositiveOverride`, `allowWithJustification`, `allowWithoutJustification`.|
|policyTip|String|**TODO: Add Description**|
|recipients|String collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

