---
title: "managedIOSLobApp resource type"
description: "Contains properties and inherited properties for Managed iOS Line Of Business apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedIOSLobApp resource type

Contains properties and inherited properties for Managed iOS Line Of Business apps.


Inherits from [managedMobileLobApp](../resources/managedMobileLobApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedIOSLobApps](../api/managedioslobapp-list.md)|[managedIOSLobApp](../resources/managedIOSLobApp.md) collection|List properties and relationships of the [managedIOSLobApp](../resources/managedioslobapp.md) objects.|
|[Get managedIOSLobApp](../api/managedioslobapp-get.md)|[managedIOSLobApp](../resources/managedIOSLobApp.md)|Read properties and relationships of the [managedIOSLobApp](../resources/managedioslobapp.md) object.|
|[Create managedIOSLobApp](../api/managedioslobapp-create.md)|[managedIOSLobApp](../resources/managedIOSLobApp.md)|Create a new [managedIOSLobApp](../resources/managedioslobapp.md) object.|
|[Delete managedIOSLobApp](../api/managedioslobapp-delete.md)|None|Deletes a [managedIOSLobApp](../resources/managedioslobapp.md).|
|[Update managedIOSLobApp](../api/managedioslobapp-update.md)|[managedIOSLobApp](../resources/managedIOSLobApp.md)|Update the properties of a [managedIOSLobApp](../resources/managedioslobapp.md) object.|
|[List categories](../api/managedioslobapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/managedioslobapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/managedioslobapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/managedioslobapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/managedioslobapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/managedioslobapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/managedioslobapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/managedioslobapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/managedioslobapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/managedioslobapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md)|Add relationships by posting to the relationships collection.|
|[List contentVersions](../api/managedioslobapp-list-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileAppContent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/managedioslobapp-post-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileAppContent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAvailability|Enumeration|The Application's availability. Inherited from [managedApp](../resources/managedApp.md). Possible values are: `global`, `lineOfBusiness`.|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosDeviceType.md)|The iOS architecture for which this app can run on.|
|buildNumber|String|The build number of managed iOS Line of Business (LoB) app.|
|bundleId|String|The Identity Name.|
|committedContentVersion|String|The internal committed content version. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|expirationDateTime|DateTimeOffset|The expiration time.|
|fileName|String|The name of the main Lob application file. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|identityVersion|String|The identity version.|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosMinimumOperatingSystem.md)|The value for the minimum applicable operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|size|Int64|The total size, including all uploaded files. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|version|String|The Application's version. Inherited from [managedApp](../resources/managedApp.md)|
|versionNumber|String|The version number of managed iOS Line of Business (LoB) app.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|categories|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileApp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileAppContent.md) collection|The list of content versions for this app. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileApp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|List of relationships for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSLobApp",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
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
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String",
  "identityVersion": "String"
}
```

