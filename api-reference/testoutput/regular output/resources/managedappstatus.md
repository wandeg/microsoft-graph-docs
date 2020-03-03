---
title: "managedAppStatus resource type"
description: "Represents app protection and configuration status for the organization."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppStatus resource type


Namespace: microsoft.graph

Represents app protection and configuration status for the organization.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppStatuses](../api/managedappstatus-list.md)|[managedAppStatus](../resources/managedappstatus.md) collection|List properties and relationships of the [managedAppStatus](../resources/managedappstatus.md) objects.|
|[Get managedAppStatus](../api/managedappstatus-get.md)|[managedAppStatus](../resources/managedappstatus.md)|Read properties and relationships of the [managedAppStatus](../resources/managedappstatus.md) object.|
|[List managedAppStatuses](../api/deviceappmanagement-list-managedappstatuses.md)|[managedAppStatus](../resources/managedappstatus.md) collection|Get the managedAppStatuses from the managedAppStatuses navigation property.|
|[Add managedAppStatuses](../api/deviceappmanagement-post-managedappstatuses.md)|[managedAppStatus](../resources/managedappstatus.md)|Add managedAppStatuses by posting to the managedAppStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Friendly name of the status report.|
|id|String| Inherited from [entity](../resources/entity.md)|
|version|String|Version of the entity.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String"
}
```

