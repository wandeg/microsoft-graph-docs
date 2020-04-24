---
title: "privilegedOperationEvent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedOperationEvent resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedOperationEvents](../api/privilegedoperationevent-list.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md) collection|Get a list of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) objects and their properties.|
|[Get privilegedOperationEvent](../api/privilegedoperationevent-get.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md)|Read the properties and relationships of a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|
|[Create privilegedOperationEvent](../api/privilegedoperationevent-post-privilegedoperationevents.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md)|Create a new [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|
|[Delete privilegedOperationEvent](../api/privilegedoperationevent-delete.md)|None|Deletes a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|
|[Update privilegedOperationEvent](../api/privilegedoperationevent-update.md)|[privilegedOperationEvent](../resources/privilegedoperationevent.md)|Update the properties of a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|referenceKey|String|**TODO: Add Description**|
|referenceSystem|String|**TODO: Add Description**|
|requestorId|String|**TODO: Add Description**|
|requestorName|String|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|roleName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userMail|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|

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

