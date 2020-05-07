---
title: "mobileAppTroubleshootingEvent resource type"
description: "MobileAppTroubleshootingEvent Entity."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppTroubleshootingEvent resource type


Namespace: microsoft.graph

MobileAppTroubleshootingEvent Entity.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|Get the appLogCollectionRequests from the appLogCollectionRequests navigation property.|
|[Create appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Create a new appLogCollectionRequests object.|
|[Delete appLogCollectionRequests](../api/mobileapptroubleshootingevent-delete-applogcollectionrequests.md)|None|Delete an [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[Update appLogCollectionRequests](../api/mobileapptroubleshootingevent-update-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Update the properties of an appLogCollectionRequests object.|
|[Get appLogCollectionRequest](../api/applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Read the properties and relationships of an [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The GUID for the object|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|The collection property of AppLogUploadRequest.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.mobileAppTroubleshootingEvent",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.mobileAppTroubleshootingEvent",
  "id": "String (identifier)"
}
```

