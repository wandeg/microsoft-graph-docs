---
title: "managedAndroidLobApp resource type"
description: "Contains properties and inherited properties for Managed Android Line Of Business apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAndroidLobApp resource type

Contains properties and inherited properties for Managed Android Line Of Business apps.


Inherits from [managedMobileLobApp](../resources/managedMobileLobApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAndroidLobApps](../api/managedandroidlobapp-list.md)|[managedAndroidLobApp](../resources/managedAndroidLobApp.md) collection|List properties and relationships of the [managedAndroidLobApp](../resources/managedandroidlobapp.md) objects.|
|[Get managedAndroidLobApp](../api/managedandroidlobapp-get.md)|[managedAndroidLobApp](../resources/managedAndroidLobApp.md)|Read properties and relationships of the [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[Create managedAndroidLobApp](../api/managedandroidlobapp-create.md)|[managedAndroidLobApp](../resources/managedAndroidLobApp.md)|Create a new [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[Delete managedAndroidLobApp](../api/managedandroidlobapp-delete.md)|None|Deletes a [managedAndroidLobApp](../resources/managedandroidlobapp.md).|
|[Update managedAndroidLobApp](../api/managedandroidlobapp-update.md)|[managedAndroidLobApp](../resources/managedAndroidLobApp.md)|Update the properties of a [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[List categories](../api/managedandroidlobapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/managedandroidlobapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/managedandroidlobapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/managedandroidlobapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/managedandroidlobapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/managedandroidlobapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/managedandroidlobapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/managedandroidlobapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/managedandroidlobapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/managedandroidlobapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md)|Add relationships by posting to the relationships collection.|
|[List contentVersions](../api/managedandroidlobapp-list-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileAppContent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/managedandroidlobapp-post-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileAppContent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAvailability|Enumeration|The Application's availability. Inherited from [managedApp](../resources/managedApp.md). Possible values are: `global`, `lineOfBusiness`.|
|committedContentVersion|String|The internal committed content version. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|identityName|String|The Identity Name.|
|identityVersion|String|The identity version.|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidMinimumOperatingSystem.md)|The value for the minimum applicable operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|packageId|String|The package identifier.|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|size|Int64|The total size, including all uploaded files. Inherited from [managedMobileLobApp](../resources/managedMobileLobApp.md)|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|version|String|The Application's version. Inherited from [managedApp](../resources/managedApp.md)|
|versionCode|String|The version code of managed Android Line of Business (LoB) app.|
|versionName|String|The version name of managed Android Line of Business (LoB) app.|

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
  "@odata.type": "microsoft.graph.managedAndroidLobApp",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "String",
  "identityName": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "String",
  "versionCode": "String",
  "identityVersion": "String"
}
```

