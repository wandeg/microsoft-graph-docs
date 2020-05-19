---
title: "managedAppStatusRaw resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAppStatusRaw resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managedAppStatus](../resources/managedappstatus.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description** Inherited from [managedAppStatus](../resources/intune-managedappstatus.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppStatus](../resources/intune-managedappstatus.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

