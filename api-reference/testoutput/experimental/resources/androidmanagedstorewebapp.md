---
title: "androidManagedStoreWebApp resource type"
description: "Contains properties and inherited properties for web apps configured to be distributed via the managed Android app store."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# androidManagedStoreWebApp resource type

Contains properties and inherited properties for web apps configured to be distributed via the managed Android app store.


Inherits from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidManagedStoreWebApps](../api/androidmanagedstorewebapp-list.md)|[androidManagedStoreWebApp](../resources/androidManagedStoreWebApp.md) collection|List properties and relationships of the [androidManagedStoreWebApp](../resources/androidmanagedstorewebapp.md) objects.|
|[Get androidManagedStoreWebApp](../api/androidmanagedstorewebapp-get.md)|[androidManagedStoreWebApp](../resources/androidManagedStoreWebApp.md)|Read properties and relationships of the [androidManagedStoreWebApp](../resources/androidmanagedstorewebapp.md) object.|
|[Create androidManagedStoreWebApp](../api/androidmanagedstorewebapp-create.md)|[androidManagedStoreWebApp](../resources/androidManagedStoreWebApp.md)|Create a new [androidManagedStoreWebApp](../resources/androidmanagedstorewebapp.md) object.|
|[Delete androidManagedStoreWebApp](../api/androidmanagedstorewebapp-delete.md)|None|Deletes a [androidManagedStoreWebApp](../resources/androidmanagedstorewebapp.md).|
|[Update androidManagedStoreWebApp](../api/androidmanagedstorewebapp-update.md)|[androidManagedStoreWebApp](../resources/androidManagedStoreWebApp.md)|Update the properties of a [androidManagedStoreWebApp](../resources/androidmanagedstorewebapp.md) object.|
|[List categories](../api/androidmanagedstorewebapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/androidmanagedstorewebapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/androidmanagedstorewebapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/androidmanagedstorewebapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/androidmanagedstorewebapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidmanagedstorewebapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidmanagedstorewebapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidmanagedstorewebapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/androidmanagedstorewebapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/androidmanagedstorewebapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md)|Add relationships by posting to the relationships collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|String|The Identity Name. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|appStoreUrl|String|The Play for Work Store app URL. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isPrivate|Boolean|Indicates whether the app is only available to a given enterprise's users. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|isSystemApp|Boolean|Indicates whether the app is a preinstalled system app. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|packageId|String|The package identifier. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|supportsOemConfig|Boolean|Whether this app supports OEMConfig policy. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|totalLicenseCount|Int32|The total number of VPP licenses. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|usedLicenseCount|Int32|The number of VPP licenses in use. Inherited from [androidManagedStoreApp](../resources/androidManagedStoreApp.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|categories|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileApp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileApp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|List of relationships for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileApp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreWebApp",
  "baseType": "microsoft.graph.androidManagedStoreApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "String",
  "appIdentifier": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "appStoreUrl": "String",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

