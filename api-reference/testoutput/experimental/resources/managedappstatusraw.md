---
title: "managedAppStatusRaw resource type"
description: "Represents an un-typed status report about organizations app protection and configuration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppStatusRaw resource type


Namespace: microsoft.graph

Represents an un-typed status report about organizations app protection and configuration.


Inherits from [managedAppStatus](../resources/managedappstatus.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppStatusRaws](../api/managedappstatusraw-list.md)|[managedAppStatusRaw](../resources/managedappstatusraw.md) collection|List properties and relationships of the [managedAppStatusRaw](../resources/managedappstatusraw.md) objects.|
|[Get managedAppStatusRaw](../api/managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/managedappstatusraw.md)|Read properties and relationships of the [managedAppStatusRaw](../resources/managedappstatusraw.md) object.|
|[Create managedAppStatusRaw](../api/managedappstatusraw-create.md)|[managedAppStatusRaw](../resources/managedappstatusraw.md)|Create a new [managedAppStatusRaw](../resources/managedappstatusraw.md) object.|
|[Delete managedAppStatusRaw](../api/managedappstatusraw-delete.md)|None|Deletes a [managedAppStatusRaw](../resources/managedappstatusraw.md).|
|[Update managedAppStatusRaw](../api/managedappstatusraw-update.md)|[managedAppStatusRaw](../resources/managedappstatusraw.md)|Update the properties of a [managedAppStatusRaw](../resources/managedappstatusraw.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|[Json](../resources/json.md)|Status report content.|
|displayName|String|Friendly name of the status report. Inherited from [managedAppStatus](../resources/managedappstatus.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|version|String|Version of the entity. Inherited from [managedAppStatus](../resources/managedappstatus.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw",
  "baseType": "microsoft.graph.managedAppStatus",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

