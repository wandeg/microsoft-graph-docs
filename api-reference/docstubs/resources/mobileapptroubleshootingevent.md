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


Inherits from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Read the properties and relationships of a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[Update mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Update the properties of a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|Get the appLogCollectionRequests from the appLogCollectionRequests navigation property.|
|[Create appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Create a new appLogCollectionRequests object.|
|[Delete appLogCollectionRequests](../api/mobileapptroubleshootingevent-delete-applogcollectionrequests.md)|None|Delete an [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|
|[Update appLogCollectionRequests](../api/mobileapptroubleshootingevent-update-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Update the properties of an appLogCollectionRequests object.|
|[Get appLogCollectionRequest](../api/applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/applogcollectionrequest.md)|Read the properties and relationships of an [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|applicationId|String|Intune application identifier.|
|correlationId|String|Id used for tracing the failure in the service. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred . Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventName|String|Event Name corresponding to the Troubleshooting Event. It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|history|[mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md) collection|Intune Mobile Application Troubleshooting History Item|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|Object containing detailed information about the error and its remediation. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|userId|String|Identifier for the user that tried to enroll the device.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/applogcollectionrequest.md) collection|The collection property of AppLogUploadRequest.|

## JSON representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```

