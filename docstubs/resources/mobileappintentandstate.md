---
title: "mobileAppIntentAndState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppIntentAndState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppIntentAndState](../api/mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Read properties and relationships of the [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|
|[Update mobileAppIntentAndState](../api/mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/mobileappintentandstate.md)|Update the properties of a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String||
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/mobileappintentandstatedetail.md) collection||
|userId|String||

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

