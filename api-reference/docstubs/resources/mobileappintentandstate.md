---
title: "mobileAppIntentAndState resource type"
description: "MobileApp Intent and Install State for a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppIntentAndState resource type


Namespace: microsoft.graph

MobileApp Intent and Install State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppIntentAndState](../api/mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Read the properties and relationships of a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|
|[Update mobileAppIntentAndState](../api/mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Update the properties of a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/mobileappintentandstatedetail.md) collection|The list of payload intents and states for the tenant.|
|userId|String|Identifier for the user that tried to enroll the device.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
    }
  ]
}
```

