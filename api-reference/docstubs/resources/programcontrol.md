---
title: "programControl resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# programControl resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List programControls](../api/programcontrol-list.md)|[programControl](../resources/programcontrol.md) collection|Get a list of the [programControl](../resources/programcontrol.md) objects and their properties.|
|[Get programControl](../api/programcontrol-get.md)|[programControl](../resources/programcontrol.md)|Read properties and relationships of a [programControl](../resources/programcontrol.md) object.|
|[Create programControl](../api/programcontrol-post-programcontrols.md)|[programControl](../resources/programcontrol.md)|Create a new [programControl](../resources/programcontrol.md) object.|
|[Delete programControl](../api/programcontrol-delete.md)|None|Deletes a [programControl](../resources/programcontrol.md).|
|[Update programControl](../api/programcontrol-update.md)|[programControl](../resources/programcontrol.md)|Update the properties of a [programControl](../resources/programcontrol.md) object.|
|[List program](../api/programcontrol-list-program.md)|[program](../resources/program.md) collection|Get the programs from the program navigation property.|
|[Create program](../api/programcontrol-post-program.md)|[program](../resources/program.md)|Create a new program object.|
|[Delete program](../api/programcontrol-delete-program.md)|None|Delete a program object.|
|[Update program](../api/programcontrol-update-program.md)|[program](../resources/program.md)|Update the properties of a program object.|
|[Get program](../api/program-get.md)|[program](../resources/program.md)|Read properties and relationships of a [program](../resources/program.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|controlId|String|**TODO: Add Description**|
|controlTypeId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|owner|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|programId|String|**TODO: Add Description**|
|resource|[programResource](../resources/programresource.md)|**TODO: Add Description**|
|status|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|program|[program](../resources/program.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.programControl",
  "baseType": "",
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

