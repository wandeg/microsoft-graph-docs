---
title: "appLogCollectionRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appLogCollectionRequest resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appLogCollectionRequest](../api/applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Read properties and relationships of the [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[Update appLogCollectionRequest](../api/applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Update the properties of a [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[createDownloadUrl](../api/applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/applogcollectiondownloaddetails.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset||
|customLogFolders|String collection||
|errorMessage|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Possible values are: `pending`, `completed`, `failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```

