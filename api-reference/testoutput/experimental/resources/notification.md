---
title: "notification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# notification resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get notification](../api/notification-get.md)|[notification](../resources/notification.md)|Read properties and relationships of the [notification](../resources/notification.md) object.|
|[Update notification](../api/notification-update.md)|[notification](../resources/notification.md)|Update the properties of a [notification](../resources/notification.md) object.|
|[List notifications](../api/user-list-notifications.md)|[notification](../resources/notification.md) collection|Get the notifications from the notifications navigation property.|
|[Add notifications](../api/user-post-notifications.md)|[notification](../resources/notification.md)|Add notifications by posting to the notifications collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayTimeToLive|Int32||
|expirationDateTime|DateTimeOffset||
|groupName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|payload|[payloadTypes](../resources/payloadtypes.md)||
|priority|Enumeration|. Possible values are: `None`, `High`, `Low`.|
|targetHostName|String||
|targetPolicy|[targetPolicyEndpoints](../resources/targetpolicyendpoints.md)||

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

