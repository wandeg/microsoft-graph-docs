---
title: "privilegedOperationEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# privilegedOperationEvent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedOperationEvents](../api/privilegedoperationevent-list.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md) collection|List properties and relationships of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) objects.|
|[Get privilegedOperationEvent](../api/privilegedoperationevent-get.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md)|Read properties and relationships of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|
|[Create privilegedOperationEvent](../api/privilegedoperationevent-post-privilegedoperationevents.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md)|Create a new [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|
|[Delete privilegedOperationEvent](../api/privilegedoperationevent-delete.md)|None|Deletes a [privilegedOperationEvent](../resources/privilegedoperationevent.md).|
|[Update privilegedOperationEvent](../api/privilegedoperationevent-update.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md)|Update the properties of a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|String||
|creationDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|referenceKey|String||
|referenceSystem|String||
|requestorId|String||
|requestorName|String||
|requestType|String||
|roleId|String||
|roleName|String||
|tenantId|String||
|userId|String||
|userMail|String||
|userName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "userMail": "String",
  "roleId": "String",
  "roleName": "String",
  "expirationDateTime": "String (timestamp)",
  "creationDateTime": "String (timestamp)",
  "requestorId": "String",
  "requestorName": "String",
  "tenantId": "String",
  "requestType": "String",
  "additionalInformation": "String",
  "referenceKey": "String",
  "referenceSystem": "String"
}
```

