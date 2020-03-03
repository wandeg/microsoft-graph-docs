---
title: "deviceCategory resource type"
description: "Device categories provides a way to organize your devices. Using device categories, company administrators can define their own categories that make sense to their company. These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment. You can filter reports and create dynamic Azure Active Directory device groups based on device categories."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceCategory resource type

Device categories provides a way to organize your devices. Using device categories, company administrators can define their own categories that make sense to their company. These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment. You can filter reports and create dynamic Azure Active Directory device groups based on device categories.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/deviceCategory.md)|Read properties and relationships of the [deviceCategory](../resources/devicecategory.md) object.|
|[Delete deviceCategory](../api/devicecategory-delete.md)|None|Deletes a [deviceCategory](../resources/devicecategory.md).|
|[Update deviceCategory](../api/devicecategory-update.md)|[deviceCategory](../resources/deviceCategory.md)|Update the properties of a [deviceCategory](../resources/devicecategory.md) object.|
|[List deviceCategories](../api/intune-devices-devicemanagement-list-devicecategories.md)|[deviceCategory](../resources/deviceCategory.md) collection|Get the deviceCategories from the deviceCategories navigation property.|
|[Add deviceCategories](../api/intune-devices-devicemanagement-post-devicecategories.md)|[deviceCategory](../resources/deviceCategory.md)|Add deviceCategories by posting to the deviceCategories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Optional description for the device category.|
|displayName|String|Display name for the device category.|
|id|String| Inherited from [entity](../resources/entity.md)|
|roleScopeTagIds|String collection|Optional role scope tags for the device category.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

