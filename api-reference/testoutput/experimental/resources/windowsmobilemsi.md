---
title: "windowsMobileMSI resource type"
description: "Contains properties and inherited properties for Windows Mobile MSI Line Of Business apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsMobileMSI resource type

Contains properties and inherited properties for Windows Mobile MSI Line Of Business apps.


Inherits from [mobileLobApp](../resources/mobileLobApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsMobileMSIs](../api/windowsmobilemsi-list.md)|[windowsMobileMSI](../resources/windowsMobileMSI.md) collection|List properties and relationships of the [windowsMobileMSI](../resources/windowsmobilemsi.md) objects.|
|[Get windowsMobileMSI](../api/windowsmobilemsi-get.md)|[windowsMobileMSI](../resources/windowsMobileMSI.md)|Read properties and relationships of the [windowsMobileMSI](../resources/windowsmobilemsi.md) object.|
|[Create windowsMobileMSI](../api/windowsmobilemsi-create.md)|[windowsMobileMSI](../resources/windowsMobileMSI.md)|Create a new [windowsMobileMSI](../resources/windowsmobilemsi.md) object.|
|[Delete windowsMobileMSI](../api/windowsmobilemsi-delete.md)|None|Deletes a [windowsMobileMSI](../resources/windowsmobilemsi.md).|
|[Update windowsMobileMSI](../api/windowsmobilemsi-update.md)|[windowsMobileMSI](../resources/windowsMobileMSI.md)|Update the properties of a [windowsMobileMSI](../resources/windowsmobilemsi.md) object.|
|[List categories](../api/windowsmobilemsi-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/windowsmobilemsi-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/windowsmobilemsi-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsmobilemsi-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/windowsmobilemsi-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowsmobilemsi-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windowsmobilemsi-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windowsmobilemsi-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/windowsmobilemsi-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/windowsmobilemsi-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md)|Add relationships by posting to the relationships collection.|
|[List contentVersions](../api/windowsmobilemsi-list-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileAppContent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Add contentVersions](../api/windowsmobilemsi-post-contentversions.md)|[mobileAppContent](../resources/intune-apps-mobileAppContent.md)|Add contentVersions by posting to the contentVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|commandLine|String|The command line.|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|identityVersion|String|The identity version.|
|ignoreVersionDetection|Boolean|A boolean to control whether the app's version will be used to detect the app after it is installed on a device. Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|productCode|String|The product code.|
|productVersion|String|The product version of Windows Mobile MSI Line of Business (LoB) app.|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|useDeviceContext|Boolean|Indicates whether to install a dual-mode MSI in the device context. If true, app will be installed for all users. If false, app will be installed per-user. If null, service will use the MSI package's default install context. In case of dual-mode MSI, this default will be per-user.  Cannot be set for non-dual-mode apps.  Cannot be changed after initial creation of the application.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|categories|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileApp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileAppContent.md) collection|The list of content versions for this app. Inherited from [mobileLobApp](../resources/mobileLobApp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileApp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|List of relationships for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|

## JSON Representation
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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true,
  "identityVersion": "String",
  "useDeviceContext": true
}
```

