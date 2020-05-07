---
title: "notification resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# notification resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayTimeToLive|Int32|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|groupName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|payload|[payloadTypes](../resources/payloadtypes.md)|**TODO: Add Description**|
|priority|priority|**TODO: Add Description**. Possible values are: `None`, `High`, `Low`.|
|targetHostName|String|**TODO: Add Description**|
|targetPolicy|[targetPolicyEndpoints](../resources/targetpolicyendpoints.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notification",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notification",
  "id": "String (identifier)",
  "targetHostName": "String",
  "expirationDateTime": "String (timestamp)",
  "payload": {
    "@odata.type": "microsoft.graph.payloadTypes"
  },
  "displayTimeToLive": "Integer",
  "priority": "String",
  "groupName": "String",
  "targetPolicy": {
    "@odata.type": "microsoft.graph.targetPolicyEndpoints"
  }
}
```

