---
title: "appliedConditionalAccessPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# appliedConditionalAccessPolicy resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conditionsNotSatisfied|conditionalAccessConditions|**TODO: Add Description**. Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|conditionsSatisfied|conditionalAccessConditions|**TODO: Add Description**. Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|displayName|String|**TODO: Add Description**|
|enforcedGrantControls|String collection|**TODO: Add Description**|
|enforcedSessionControls|String collection|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|result|appliedConditionalAccessPolicyResult|**TODO: Add Description**. Possible values are: `success`, `failure`, `notApplied`, `notEnabled`, `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.appliedConditionalAccessPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "enforcedGrantControls": [
    "String"
  ],
  "enforcedSessionControls": [
    "String"
  ],
  "conditionsSatisfied": "String",
  "conditionsNotSatisfied": "String",
  "result": "String"
}
```

