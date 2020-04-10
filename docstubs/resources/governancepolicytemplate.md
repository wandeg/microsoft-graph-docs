---
title: "governancePolicyTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governancePolicyTemplate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get governancePolicyTemplate](../api/governancepolicytemplate-get.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Read properties and relationships of the [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.|
|[Update governancePolicyTemplate](../api/governancepolicytemplate-update.md)|[governancePolicyTemplate](../resources/governancepolicytemplate.md)|Update the properties of a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|policy|[governancePolicy](../resources/governancepolicy.md)||
|settings|[businessFlowSettings](../resources/businessflowsettings.md)||

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

