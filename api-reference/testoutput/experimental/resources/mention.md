---
title: "mention resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mention resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mention](../api/mention-get.md)|[mention](../resources/mention.md)|Read properties and relationships of the [mention](../resources/mention.md) object.|
|[Delete mention](../api/mention-delete.md)|None|Deletes a [mention](../resources/mention.md).|
|[Update mention](../api/mention-update.md)|[mention](../resources/mention.md)|Update the properties of a [mention](../resources/mention.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|application|String||
|clientReference|String||
|createdBy|[emailAddress](../resources/emailAddress.md)||
|createdDateTime|DateTimeOffset||
|deepLink|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|mentioned|[emailAddress](../resources/emailAddress.md)||
|mentionText|String||
|serverCreatedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mention",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mention",
  "id": "String (identifier)",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "mentionText": "String",
  "clientReference": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "createdDateTime": "String (timestamp)",
  "serverCreatedDateTime": "String (timestamp)",
  "deepLink": "String",
  "application": "String"
}
```

