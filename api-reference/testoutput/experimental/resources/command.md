---
title: "command resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# command resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List commands](../api/command-list.md)|[command](../resources/command.md) collection|List properties and relationships of the [command](../resources/command.md) objects.|
|[Get command](../api/command-get.md)|[command](../resources/command.md)|Read properties and relationships of the [command](../resources/command.md) object.|
|[Create command](../api/command-post-commands.md)|[command](../resources/command.md)|Create a new [command](../resources/command.md) object.|
|[Delete command](../api/command-delete.md)|None|Deletes a [command](../resources/command.md).|
|[Update command](../api/command-update.md)|[command](../resources/command.md)|Update the properties of a [command](../resources/command.md) object.|
|[Get payloadResponse](../api/payloadresponse-get.md)|[payloadResponse](../resources/payloadresponse.md)|Read properties and relationships of the [payloadResponse](../resources/payloadresponse.md) object.|
|[List commands](../api/device-list-commands.md)|[command](../resources/command.md) collection|Get the commands from the commands navigation property.|
|[Add commands](../api/device-post-commands.md)|[command](../resources/command.md)|Add commands by posting to the commands collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|AppServiceName|String||
|Error|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|PackageFamilyName|String||
|Payload|[PayloadRequest](../resources/payloadrequest.md)||
|PermissionTicket|String||
|PostBackUri|String||
|Status|String||
|Type|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|responsepayload|[payloadResponse](../resources/payloadresponse.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.command",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.command",
  "id": "String (identifier)",
  "Status": "String",
  "Type": "String",
  "AppServiceName": "String",
  "PackageFamilyName": "String",
  "Error": "String",
  "Payload": {
    "@odata.type": "microsoft.graph.PayloadRequest"
  },
  "PermissionTicket": "String",
  "PostBackUri": "String"
}
```

