---
title: "programControl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# programControl resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List programControls](../api/programcontrol-list.md)|[programControl](../resources/programcontrol.md) collection|List properties and relationships of the [programControl](../resources/programcontrol.md) objects.|
|[Get programControl](../api/programcontrol-get.md)|[programControl](../resources/programcontrol.md)|Read properties and relationships of the [programControl](../resources/programcontrol.md) object.|
|[Create programControl](../api/programcontrol-post-programcontrols.md)|[programControl](../resources/programcontrol.md)|Create a new [programControl](../resources/programcontrol.md) object.|
|[Delete programControl](../api/programcontrol-delete.md)|None|Deletes a [programControl](../resources/programcontrol.md).|
|[Update programControl](../api/programcontrol-update.md)|[programControl](../resources/programcontrol.md)|Update the properties of a [programControl](../resources/programcontrol.md) object.|
|[Get program](../api/program-get.md)|[program](../resources/program.md)|Read properties and relationships of the [program](../resources/program.md) object.|
|[List controls](../api/program-list-controls.md)|[programControl](../resources/programcontrol.md) collection|Get the programControls from the controls navigation property.|
|[Add controls](../api/program-post-controls.md)|[programControl](../resources/programcontrol.md)|Add controls by posting to the controls collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|controlId|String||
|controlTypeId|String||
|createdDateTime|DateTimeOffset||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|owner|[userIdentity](../resources/useridentity.md)||
|programId|String||
|resource|[programResource](../resources/programresource.md)||
|status|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|program|[program](../resources/program.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.programControl",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.programControl",
  "id": "String (identifier)",
  "controlId": "String",
  "programId": "String",
  "controlTypeId": "String",
  "displayName": "String",
  "status": "String",
  "owner": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "String",
    "ipAddress": "String",
    "userPrincipalName": "String"
  },
  "resource": {
    "@odata.type": "microsoft.graph.programResource",
    "type": "String"
  },
  "createdDateTime": "String (timestamp)"
}
```

