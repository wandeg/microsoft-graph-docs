---
title: "iosStoreApp resource type"
description: "Contains properties and inherited properties for iOS store apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosStoreApp resource type


Namespace: microsoft.graph

Contains properties and inherited properties for iOS store apps.


Inherits from [mobileApp](../resources/mobileapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosStoreApps](../api/iosstoreapp-list.md)|[iosStoreApp](../resources/iosstoreapp.md) collection|List properties and relationships of the [iosStoreApp](../resources/iosstoreapp.md) objects.|
|[Get iosStoreApp](../api/iosstoreapp-get.md)|[iosStoreApp](../resources/iosstoreapp.md)|Read properties and relationships of the [iosStoreApp](../resources/iosstoreapp.md) object.|
|[Create iosStoreApp](../api/iosstoreapp-create.md)|[iosStoreApp](../resources/iosstoreapp.md)|Create a new [iosStoreApp](../resources/iosstoreapp.md) object.|
|[Delete iosStoreApp](../api/iosstoreapp-delete.md)|None|Deletes a [iosStoreApp](../resources/iosstoreapp.md).|
|[Update iosStoreApp](../api/iosstoreapp-update.md)|[iosStoreApp](../resources/iosstoreapp.md)|Update the properties of a [iosStoreApp](../resources/iosstoreapp.md) object.|
|[assign](../api/iosstoreapp-assign.md)|None||
|[List categories](../api/iosstoreapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/iosstoreapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/iosstoreapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/iosstoreapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableDeviceType|[iosDeviceType](../resources/iosdevicetype.md)|The iOS architecture for which this app can run on.|
|appStoreUrl|String|The Apple App Store URL|
|bundleId|String|The Identity Name.|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md)|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md)|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/iosminimumoperatingsystem.md)|The value for the minimum applicable operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosStoreApp",
  "baseType": "microsoft.graph.mobileApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "bundleId": "String",
  "appStoreUrl": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```

