---
title: "chatMessageHostedContent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# chatMessageHostedContent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get chatMessageHostedContent](../api/chatmessagehostedcontent-get.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Read properties and relationships of the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.|
|[Update chatMessageHostedContent](../api/chatmessagehostedcontent-update.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Update the properties of a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.|
|[List hostedContents](../api/chatmessage-list-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|Get the chatMessageHostedContents from the hostedContents navigation property.|
|[Add hostedContents](../api/chatmessage-post-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Add hostedContents by posting to the hostedContents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageHostedContent",
  "id": "String (identifier)"
}
```

