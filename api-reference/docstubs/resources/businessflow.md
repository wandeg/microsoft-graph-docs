---
title: "businessFlow resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# businessFlow resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get businessFlow](../api/businessflow-get.md)|[businessFlow](../resources/businessflow.md)|Read properties and relationships of a [businessFlow](../resources/businessflow.md) object.|
|[Update businessFlow](../api/businessflow-update.md)|[businessFlow](../resources/businessflow.md)|Update the properties of a [businessFlow](../resources/businessflow.md) object.|
|[recordDecisions](../api/businessflow-recorddecisions.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customData|String|**TODO: Add Description**|
|deDuplicationId|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|policy|[governancePolicy](../resources/governancepolicy.md)|**TODO: Add Description**|
|policyTemplateId|String|**TODO: Add Description**|
|recordVersion|String|**TODO: Add Description**|
|schemaId|String|**TODO: Add Description**|
|settings|[businessFlowSettings](../resources/businessflowsettings.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.businessFlow",
  "baseType": "",
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

