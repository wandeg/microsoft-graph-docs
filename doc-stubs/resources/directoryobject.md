---
title: "directoryObject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# directoryObject resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[getByIds](../api/directoryobject-getbyids.md)|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/directoryobject-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[validateProperties](../api/directoryobject-validateproperties.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "baseType": "",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)"
}
```

