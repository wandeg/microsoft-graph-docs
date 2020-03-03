---
title: "windowsUniversalAppX resource type"
description: "Contains properties and inherited properties for Windows Universal AppX Line Of Business apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsUniversalAppX resource type

Contains properties and inherited properties for Windows Universal AppX Line Of Business apps.


Inherits from [mobileLobApp](../resources/mobileLobApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsUniversalAppXs](../api/windowsuniversalappx-list.md)|[windowsUniversalAppX](../resources/windowsUniversalAppX.md) collection|List properties and relationships of the [windowsUniversalAppX](../resources/windowsuniversalappx.md) objects.|
|[Get windowsUniversalAppX](../api/windowsuniversalappx-get.md)|[windowsUniversalAppX](../resources/windowsUniversalAppX.md)|Read properties and relationships of the [windowsUniversalAppX](../resources/windowsuniversalappx.md) object.|
|[Create windowsUniversalAppX](../api/windowsuniversalappx-create.md)|[windowsUniversalAppX](../resources/windowsUniversalAppX.md)|Create a new [windowsUniversalAppX](../resources/windowsuniversalappx.md) object.|
|[Delete windowsUniversalAppX](../api/windowsuniversalappx-delete.md)|None|Deletes a [windowsUniversalAppX](../resources/windowsuniversalappx.md).|
|[Update windowsUniversalAppX](../api/windowsuniversalappx-update.md)|[windowsUniversalAppX](../resources/windowsUniversalAppX.md)|Update the properties of a [windowsUniversalAppX](../resources/windowsuniversalappx.md) object.|
|[List categories](../api/windowsuniversalappx-list-categories.md)|[mobileAppCategory](../resources/mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/windowsuniversalappx-post-categories.md)|[mobileAppCategory](../resources/mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/windowsuniversalappx-list-assignments.md)|[mobileAppAssignment](../resources/mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsuniversalappx-post-assignments.md)|[mobileAppAssignment](../resources/mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[List contentVersions](../api/windowsuniversalappx-list-contentversions.md)|[mobileAppContent](../resources/mobileAppContent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/windowsuniversalappx-post-contentversions.md)|[mobileAppContent](../resources/mobileAppContent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableArchitectures|Enumeration|The Windows architecture(s) for which this app can run on. Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.|
|applicableDeviceTypes|Enumeration|The Windows device type(s) for which this app can run on. Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|identityName|String|The Identity Name.|
|identityPublisherHash|String|The Identity Publisher Hash.|
|identityResourceIdentifier|String|The Identity Resource Identifier.|
|identityVersion|String|The identity version.|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileApp.md)|
|isBundle|Boolean|Whether or not the app is a bundle.|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileApp.md)|
|largeIcon|[mimeContent](../resources/mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileApp.md)|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/windowsMinimumOperatingSystem.md)|The value for the minimum applicable operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileApp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|

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
  "@odata.type": "microsoft.graph.windowsUniversalAppX",
  "baseType": "microsoft.graph.mobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "String",
  "applicableDeviceTypes": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "String"
}
```

