---
title: "appLogCollectionRequest resource type"
description: "AppLogCollectionRequest Entity."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appLogCollectionRequest resource type


Namespace: microsoft.graph

AppLogCollectionRequest Entity.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[createDownloadUrl](../api/applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/applogcollectiondownloaddetails.md)|**TODO: Add Description**|
|[createDownloadUrl2](../api/applogcollectionrequest-createdownloadurl2.md)|[appLogCollectionDownloadDetails](../resources/applogcollectiondownloaddetails.md)|**TODO: Add Description**|
|[List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|Get the appLogCollectionRequests from the appLogCollectionRequests navigation property.|
|[Create appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Create a new appLogCollectionRequests object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|Time at which the upload log request reached a terminal state|
|customLogFolders|String collection|List of log folders. |
|errorMessage|String|Error message if any during the upload process|
|id|String|The unique Identifier. This is userId_DeviceId_AppId id.|
|status|appLogUploadState|Log upload status. Possible values are: `pending`, `completed`, `failed`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.appLogCollectionRequest",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```

