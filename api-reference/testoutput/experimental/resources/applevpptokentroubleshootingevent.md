---
title: "appleVppTokenTroubleshootingEvent resource type"
description: "Event representing an Apple Vpp Token Troubleshooting Event."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appleVppTokenTroubleshootingEvent resource type


Namespace: microsoft.graph

Event representing an Apple Vpp Token Troubleshooting Event.


Inherits from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List appleVppTokenTroubleshootingEvents](../api/applevpptokentroubleshootingevent-list.md)|[appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md) collection|List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md) objects.|
|[Get appleVppTokenTroubleshootingEvent](../api/applevpptokentroubleshootingevent-get.md)|[appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md)|Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md) object.|
|[Create appleVppTokenTroubleshootingEvent](../api/applevpptokentroubleshootingevent-create.md)|[appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md)|Create a new [appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md) object.|
|[Delete appleVppTokenTroubleshootingEvent](../api/applevpptokentroubleshootingevent-delete.md)|None|Deletes a [appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md).|
|[Update appleVppTokenTroubleshootingEvent](../api/applevpptokentroubleshootingevent-update.md)|[appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md)|Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/applevpptokentroubleshootingevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|correlationId|String|Id used for tracing the failure in the service. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred . Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|eventName|String|Event Name corresponding to the Troubleshooting Event. It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|tokenId|String|Apple Volume Purchase Program Token Identifier.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|Object containing detailed information about the error and its remediation. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleVppTokenTroubleshootingEvent",
  "baseType": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
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
  "tokenId": "String"
}
```

