---
title: "deviceManagementTroubleshootingEvent resource type"
description: "Event representing an general failure."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementTroubleshootingEvent resource type


Namespace: microsoft.graph

Event representing an general failure.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementTroubleshootingEvent](../api/devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Read the properties and relationships of a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.|
|[Update deviceManagementTroubleshootingEvent](../api/devicemanagementtroubleshootingevent-update.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Update the properties of a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.|
|[List deviceManagementTroubleshootingEvents](../api/user-list-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) collection|Get the deviceManagementTroubleshootingEvents from the deviceManagementTroubleshootingEvents navigation property.|
|[Create deviceManagementTroubleshootingEvents](../api/user-post-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Create a new deviceManagementTroubleshootingEvents object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs which provides additional information on the Troubleshooting event|
|correlationId|String|Id used for tracing the failure in the service.|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|eventName|String|Event Name corresponding to the Troubleshooting Event. It is an Optional field|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|Object containing detailed information about the error and its remediation.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
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
  ]
}
```

