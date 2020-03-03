---
title: "androidLobApp resource type"
description: "Contains properties and inherited properties for Android Line Of Business apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# androidLobApp resource type

Contains properties and inherited properties for Android Line Of Business apps.


Inherits from [mobileLobApp](../resources/mobileLobApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidLobApps](../api/androidlobapp-list.md)|[androidLobApp](../resources/androidLobApp.md) collection|List properties and relationships of the [androidLobApp](../resources/androidlobapp.md) objects.|
|[Get androidLobApp](../api/androidlobapp-get.md)|[androidLobApp](../resources/androidLobApp.md)|Read properties and relationships of the [androidLobApp](../resources/androidlobapp.md) object.|
|[Create androidLobApp](../api/androidlobapp-create.md)|[androidLobApp](../resources/androidLobApp.md)|Create a new [androidLobApp](../resources/androidlobapp.md) object.|
|[Delete androidLobApp](../api/androidlobapp-delete.md)|None|Deletes a [androidLobApp](../resources/androidlobapp.md).|
|[Update androidLobApp](../api/androidlobapp-update.md)|[androidLobApp](../resources/androidLobApp.md)|Update the properties of a [androidLobApp](../resources/androidlobapp.md) object.|
|[List categories](../api/androidlobapp-list-categories.md)|[mobileAppCategory](../resources/mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/androidlobapp-post-categories.md)|[mobileAppCategory](../resources/mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/androidlobapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/androidlobapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[List contentVersions](../api/androidlobapp-list-contentversions.md)|[mobileAppContent](../resources/mobileAppContent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/androidlobapp-post-contentversions.md)|[mobileAppContent](../resources/mobileAppContent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileApp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileApp.md)|
|largeIcon|[mimeContent](../resources/mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileApp.md)|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/androidMinimumOperatingSystem.md)|The value for the minimum applicable operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|packageId|String|The package identifier.|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileApp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|versionCode|String|The version code of Android Line of Business (LoB) app.|
|versionName|String|The version name of Android Line of Business (LoB) app.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileAppAssignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|categories|[mobileAppCategory](../resources/mobileAppCategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileApp.md)|
|contentVersions|[mobileAppContent](../resources/mobileAppContent.md) collection|The list of content versions for this app. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidLobApp",
  "baseType": "microsoft.graph.mobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
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
  },
  "versionName": "String",
  "versionCode": "String"
}
```

