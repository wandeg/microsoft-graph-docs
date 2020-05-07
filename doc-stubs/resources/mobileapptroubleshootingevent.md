---
title: "mobileAppTroubleshootingEvent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppTroubleshootingEvent resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|Get the appLogCollectionRequests from the appLogCollectionRequests navigation property.|
|[Create appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Create a new appLogCollectionRequests object.|
|[Delete appLogCollectionRequests](../api/mobileapptroubleshootingevent-delete-applogcollectionrequests.md)|None|Delete an [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[Update appLogCollectionRequests](../api/mobileapptroubleshootingevent-update-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Update the properties of an appLogCollectionRequests object.|
|[Get appLogCollectionRequest](../api/applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Read the properties and relationships of an [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[List mobileAppTroubleshootingEvents](../api/user-list-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) collection|Get the mobileAppTroubleshootingEvents from the mobileAppTroubleshootingEvents navigation property.|
|[Create mobileAppTroubleshootingEvents](../api/user-post-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Create a new mobileAppTroubleshootingEvents object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description** Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|applicationId|String|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description** Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventName|String|**TODO: Add Description** Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|history|[mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String|**TODO: Add Description**|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|**TODO: Add Description** Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|userId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent",
  "baseType": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
    }
  ]
}
```

