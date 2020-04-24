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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get notification](../api/notification-get.md)|[notification](../resources/notification.md)|Read the properties and relationships of a [notification](../resources/notification.md) object.|
|[Update notification](../api/notification-update.md)|[notification](../resources/notification.md)|Update the properties of a [notification](../resources/notification.md) object.|

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
None

## JSON representation
Here is a JSON representation of the resource.
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
  "displayTimeToLive": 1024,
  "priority": "String",
  "groupName": "String",
  "targetPolicy": {
    "@odata.type": "microsoft.graph.targetPolicyEndpoints"
  }
}
```

