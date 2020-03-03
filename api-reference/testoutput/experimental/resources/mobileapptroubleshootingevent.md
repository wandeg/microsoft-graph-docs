---
title: "mobileAppTroubleshootingEvent resource type"
description: "MobileAppTroubleshootingEvent Entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppTroubleshootingEvent resource type


Namespace: microsoft.graph

MobileAppTroubleshootingEvent Entity.


Inherits from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppTroubleshootingEvents](../api/mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) collection|List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) objects.|
|[Get mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[Create mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Create a new [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[Delete mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-delete.md)|None|Deletes a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md).|
|[Update mobileAppTroubleshootingEvent](../api/mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md)|Update the properties of a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.|
|[List appLogCollectionRequests](../api/mobileapptroubleshootingevent-list-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection|Get the appLogCollectionRequests from the appLogCollectionRequests navigation property.|
|[Add appLogCollectionRequests](../api/mobileapptroubleshootingevent-post-applogcollectionrequests.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Add appLogCollectionRequests by posting to the appLogCollectionRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|applicationId|String|Intune application identifier.|
|correlationId|String|Id used for tracing the failure in the service. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred . Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventName|String|Event Name corresponding to the Troubleshooting Event. It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|history|[mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md) collection|Intune Mobile Application Troubleshooting History Item|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|Object containing detailed information about the error and its remediation. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|userId|String|Identifier for the user that tried to enroll the device.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection|The collection property of AppLogUploadRequest.|

## JSON Representation
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

