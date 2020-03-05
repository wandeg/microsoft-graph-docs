---
title: "managedAndroidStoreApp resource type"
description: "Contains properties and inherited properties for Android store apps that you can manage with an Intune app protection policy."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAndroidStoreApp resource type


Namespace: microsoft.graph

Contains properties and inherited properties for Android store apps that you can manage with an Intune app protection policy.


Inherits from [managedApp](../resources/managedapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAndroidStoreApps](../api/managedandroidstoreapp-list.md)|[managedAndroidStoreApp](../resources/managedandroidstoreapp.md) collection|List properties and relationships of the [managedAndroidStoreApp](../resources/managedandroidstoreapp.md) objects.|
|[Get managedAndroidStoreApp](../api/managedandroidstoreapp-get.md)|[managedAndroidStoreApp](../resources/managedandroidstoreapp.md)|Read properties and relationships of the [managedAndroidStoreApp](../resources/managedandroidstoreapp.md) object.|
|[Create managedAndroidStoreApp](../api/managedandroidstoreapp-create.md)|[managedAndroidStoreApp](../resources/managedandroidstoreapp.md)|Create a new [managedAndroidStoreApp](../resources/managedandroidstoreapp.md) object.|
|[Delete managedAndroidStoreApp](../api/managedandroidstoreapp-delete.md)|None|Deletes a [managedAndroidStoreApp](../resources/managedandroidstoreapp.md).|
|[Update managedAndroidStoreApp](../api/managedandroidstoreapp-update.md)|[managedAndroidStoreApp](../resources/managedandroidstoreapp.md)|Update the properties of a [managedAndroidStoreApp](../resources/managedandroidstoreapp.md) object.|
|[List categories](../api/managedandroidstoreapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/managedandroidstoreapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/managedandroidstoreapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/managedandroidstoreapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAvailability|Enumeration|The Application's availability. Inherited from [managedApp](../resources/managedapp.md). Possible values are: `global`, `lineOfBusiness`.|
|appStoreUrl|String|The Android AppStoreUrl.|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md)|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md)|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/androidminimumoperatingsystem.md)|The value for the minimum supported operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|packageId|String|The app's package ID.|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|version|String|The Application's version. Inherited from [managedApp](../resources/managedapp.md)|

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
  "@odata.type": "microsoft.graph.managedAndroidStoreApp",
  "baseType": "microsoft.graph.managedApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "String",
  "version": "String",
  "packageId": "String",
  "appStoreUrl": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

