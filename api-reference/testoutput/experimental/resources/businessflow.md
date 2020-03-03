---
title: "businessFlow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# businessFlow resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get businessFlow](../api/businessflow-get.md)|[businessFlow](../resources/businessFlow.md)|Read properties and relationships of the [businessFlow](../resources/businessflow.md) object.|
|[Delete businessFlow](../api/businessflow-delete.md)|None|Deletes a [businessFlow](../resources/businessflow.md).|
|[Update businessFlow](../api/businessflow-update.md)|[businessFlow](../resources/businessFlow.md)|Update the properties of a [businessFlow](../resources/businessflow.md) object.|
|[recordDecisions](../api/businessflow-recorddecisions.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customData|String||
|deDuplicationId|String||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|policy|[governancePolicy](../resources/governancePolicy.md)||
|policyTemplateId|String||
|recordVersion|String||
|schemaId|String||
|settings|[businessFlowSettings](../resources/businessFlowSettings.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.businessFlow",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.businessFlow",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "deDuplicationId": "String",
  "schemaId": "String",
  "customData": "String",
  "recordVersion": "String",
  "policy": {
    "@odata.type": "microsoft.graph.governancePolicy"
  },
  "policyTemplateId": "String",
  "settings": {
    "@odata.type": "microsoft.graph.businessFlowSettings"
  }
}
```

