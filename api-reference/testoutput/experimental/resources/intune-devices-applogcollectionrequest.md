---
title: "appLogCollectionRequest resource type"
description: "AppLogCollectionRequest Entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# appLogCollectionRequest resource type

AppLogCollectionRequest Entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-appLogCollectionRequest.md)|Read properties and relationships of the [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[Delete appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|None|Deletes a [appLogCollectionRequest](../resources/applogcollectionrequest.md).|
|[Update appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-appLogCollectionRequest.md)|Update the properties of a [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[createDownloadUrl](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-appLogCollectionDownloadDetails.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|Time at which the upload log request reached a terminal state|
|customLogFolders|String collection|List of log folders. |
|errorMessage|String|Error message if any during the upload process|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|Log upload status. Possible values are: `pending`, `completed`, `failed`.|

## Relationships
None

## JSON Representation
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

