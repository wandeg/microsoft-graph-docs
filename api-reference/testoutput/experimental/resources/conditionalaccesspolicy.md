---
title: "conditionalAccessPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessPolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List conditionalAccessPolicies](../api/conditionalaccesspolicy-list.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|List properties and relationships of the [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.|
|[Get conditionalAccessPolicy](../api/conditionalaccesspolicy-get.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Read properties and relationships of the [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Create conditionalAccessPolicy](../api/conditionalaccesspolicy-create.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Delete conditionalAccessPolicy](../api/conditionalaccesspolicy-delete.md)|None|Deletes a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).|
|[Update conditionalAccessPolicy](../api/conditionalaccesspolicy-update.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conditions|[conditionalAccessConditionSet](../resources/conditionalaccessconditionset.md)||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|grantControls|[conditionalAccessGrantControls](../resources/conditionalaccessgrantcontrols.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset||
|sessionControls|[conditionalAccessSessionControls](../resources/conditionalaccesssessioncontrols.md)||
|state|Enumeration|. Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "state": "String",
  "conditions": {
    "@odata.type": "microsoft.graph.conditionalAccessConditionSet"
  },
  "grantControls": {
    "@odata.type": "microsoft.graph.conditionalAccessGrantControls"
  },
  "sessionControls": {
    "@odata.type": "microsoft.graph.conditionalAccessSessionControls"
  }
}
```

