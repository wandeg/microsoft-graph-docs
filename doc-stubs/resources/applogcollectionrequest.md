---
title: "appLogCollectionRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appLogCollectionRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[createDownloadUrl](../api/applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/applogcollectiondownloaddetails.md)|**TODO: Add Description**|
|[List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|Get the appLogCollectionRequests from the appLogCollectionRequests navigation property.|
|[Create appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Create a new appLogCollectionRequests object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|customLogFolders|String collection|**TODO: Add Description**|
|errorMessage|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|appLogUploadState|**TODO: Add Description**. Possible values are: `pending`, `completed`, `failed`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

