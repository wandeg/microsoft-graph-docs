---
title: "aadUserConversationMember resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# aadUserConversationMember resource type


Namespace: microsoft.graph




Inherits from [conversationMember](../resources/conversationmember.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List aadUserConversationMembers](../api/aaduserconversationmember-list.md)|[aadUserConversationMember](../resources/aaduserconversationmember.md) collection|List properties and relationships of the [aadUserConversationMember](../resources/aaduserconversationmember.md) objects.|
|[Get aadUserConversationMember](../api/aaduserconversationmember-get.md)|[aadUserConversationMember](../resources/aaduserconversationmember.md)|Read properties and relationships of the [aadUserConversationMember](../resources/aaduserconversationmember.md) object.|
|[Create aadUserConversationMember](../api/aaduserconversationmember-create.md)|[aadUserConversationMember](../resources/aaduserconversationmember.md)|Create a new [aadUserConversationMember](../resources/aaduserconversationmember.md) object.|
|[Delete aadUserConversationMember](../api/aaduserconversationmember-delete.md)|None|Deletes a [aadUserConversationMember](../resources/aaduserconversationmember.md).|
|[Update aadUserConversationMember](../api/aaduserconversationmember-update.md)|[aadUserConversationMember](../resources/aaduserconversationmember.md)|Update the properties of a [aadUserConversationMember](../resources/aaduserconversationmember.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String| Inherited from [conversationMember](../resources/conversationmember.md)|
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|roles|String collection| Inherited from [conversationMember](../resources/conversationmember.md)|
|userId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|user|[user](../resources/user.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "userId": "String",
  "email": "String"
}
```

