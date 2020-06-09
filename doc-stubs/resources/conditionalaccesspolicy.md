---
title: "conditionalAccessPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# conditionalAccessPolicy resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List policies](../api/conditionalaccessroot-list-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|Get the conditionalAccessPolicies from the policies navigation property.|
|[Create policies](../api/conditionalaccessroot-post-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Create a new policies object.|
|[Update policies](../api/conditionalaccessroot-update-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Update the properties of a policies object.|
|[Get policies](../api/conditionalaccessroot-get-conditionalaccesspolicy.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Read the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Delete policies](../api/conditionalaccessroot-delete-policies.md)|None|Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[List conditionalAccessPolicies](../api/conditionalaccesspolicy-list.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|Get a list of the [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects and their properties.|
|[Create conditionalAccessPolicy](../api/conditionalaccesspolicy-create.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Get conditionalAccessPolicy](../api/conditionalaccesspolicy-get.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Read the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Update conditionalAccessPolicy](../api/conditionalaccesspolicy-update.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Delete conditionalAccessPolicy](../api/conditionalaccesspolicy-delete.md)|None|Deletes a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conditions|[conditionalAccessConditionSet](../resources/conditionalaccessconditionset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|grantControls|[conditionalAccessGrantControls](../resources/conditionalaccessgrantcontrols.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|sessionControls|[conditionalAccessSessionControls](../resources/conditionalaccesssessioncontrols.md)|**TODO: Add Description**|
|state|conditionalAccessPolicyState|**TODO: Add Description**. Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

