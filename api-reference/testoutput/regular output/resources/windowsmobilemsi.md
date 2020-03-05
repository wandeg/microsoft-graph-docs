---
title: "windowsMobileMSI resource type"
description: "Contains properties and inherited properties for Windows Mobile MSI Line Of Business apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsMobileMSI resource type


Namespace: microsoft.graph

Contains properties and inherited properties for Windows Mobile MSI Line Of Business apps.


Inherits from [mobileLobApp](../resources/mobilelobapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsMobileMSIs](../api/windowsmobilemsi-list.md)|[windowsMobileMSI](../resources/windowsmobilemsi.md) collection|List properties and relationships of the [windowsMobileMSI](../resources/windowsmobilemsi.md) objects.|
|[Get windowsMobileMSI](../api/windowsmobilemsi-get.md)|[windowsMobileMSI](../resources/windowsmobilemsi.md)|Read properties and relationships of the [windowsMobileMSI](../resources/windowsmobilemsi.md) object.|
|[Create windowsMobileMSI](../api/windowsmobilemsi-create.md)|[windowsMobileMSI](../resources/windowsmobilemsi.md)|Create a new [windowsMobileMSI](../resources/windowsmobilemsi.md) object.|
|[Delete windowsMobileMSI](../api/windowsmobilemsi-delete.md)|None|Deletes a [windowsMobileMSI](../resources/windowsmobilemsi.md).|
|[Update windowsMobileMSI](../api/windowsmobilemsi-update.md)|[windowsMobileMSI](../resources/windowsmobilemsi.md)|Update the properties of a [windowsMobileMSI](../resources/windowsmobilemsi.md) object.|
|[List categories](../api/windowsmobilemsi-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/windowsmobilemsi-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/windowsmobilemsi-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsmobilemsi-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Add assignments by posting to the assignments collection.|
|[List contentVersions](../api/windowsmobilemsi-list-contentversions.md)|[mobileAppContent](../resources/mobileappcontent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/windowsmobilemsi-post-contentversions.md)|[mobileAppContent](../resources/mobileappcontent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|commandLine|String|The command line.|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ignoreVersionDetection|Boolean|A boolean to control whether the app's version will be used to detect the app after it is installed on a device. Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md)|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|productCode|String|The product code.|
|productVersion|String|The product version of Windows Mobile MSI Line of Business (LoB) app.|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/mobileappcontent.md) collection|The list of content versions for this app. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI",
  "baseType": "microsoft.graph.mobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```

