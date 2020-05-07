---
title: "driveItemVersion resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# driveItemVersion resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItemVersion](../resources/baseitemversion.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[restoreVersion](../api/driveitemversion-restoreversion.md)|None|**TODO: Add Description**|
|[List versions](../api/driveitem-list-versions.md)|[driveItemVersion](../resources/driveitemversion.md) collection|Get the driveItemVersions from the versions navigation property.|
|[Create versions](../api/driveitem-post-versions.md)|[driveItemVersion](../resources/driveitemversion.md)|Create a new versions object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|size|Int64|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "baseType": "microsoft.graph.baseItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "content": "Stream",
  "size": "Integer"
}
```

