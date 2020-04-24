---
title: "governancePolicyTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# governancePolicyTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get governancePolicyTemplate](../api/governancepolicytemplate-get.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Read the properties and relationships of a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.|
|[Update governancePolicyTemplate](../api/governancepolicytemplate-update.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Update the properties of a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|policy|[governancePolicy](../resources/governancepolicy.md)|**TODO: Add Description**|
|settings|[businessFlowSettings](../resources/businessflowsettings.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governancePolicyTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governancePolicyTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "policy": {
    "@odata.type": "microsoft.graph.governancePolicy"
  },
  "settings": {
    "@odata.type": "microsoft.graph.businessFlowSettings"
  }
}
```

