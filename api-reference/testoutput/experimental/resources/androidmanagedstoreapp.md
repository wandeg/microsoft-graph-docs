---
title: "androidManagedStoreApp resource type"
description: "Contains properties and inherited properties for Android Managed Store Apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidManagedStoreApp resource type


Namespace: microsoft.graph

Contains properties and inherited properties for Android Managed Store Apps.


Inherits from [mobileApp](../resources/mobileapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidManagedStoreApps](../api/androidmanagedstoreapp-list.md)|[androidManagedStoreApp](../resources/androidmanagedstoreapp.md) collection|List properties and relationships of the [androidManagedStoreApp](../resources/androidmanagedstoreapp.md) objects.|
|[Get androidManagedStoreApp](../api/androidmanagedstoreapp-get.md)|[androidManagedStoreApp](../resources/androidmanagedstoreapp.md)|Read properties and relationships of the [androidManagedStoreApp](../resources/androidmanagedstoreapp.md) object.|
|[Create androidManagedStoreApp](../api/androidmanagedstoreapp-create.md)|[androidManagedStoreApp](../resources/androidmanagedstoreapp.md)|Create a new [androidManagedStoreApp](../resources/androidmanagedstoreapp.md) object.|
|[Delete androidManagedStoreApp](../api/androidmanagedstoreapp-delete.md)|None|Deletes a [androidManagedStoreApp](../resources/androidmanagedstoreapp.md).|
|[Update androidManagedStoreApp](../api/androidmanagedstoreapp-update.md)|[androidManagedStoreApp](../resources/androidmanagedstoreapp.md)|Update the properties of a [androidManagedStoreApp](../resources/androidmanagedstoreapp.md) object.|
|[assign](../api/androidmanagedstoreapp-assign.md)|None||
|[updateRelationships](../api/androidmanagedstoreapp-updaterelationships.md)|None||
|[getRelatedAppStates](../api/androidmanagedstoreapp-getrelatedappstates.md)|[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection||
|[List categories](../api/androidmanagedstoreapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/androidmanagedstoreapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/androidmanagedstoreapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/androidmanagedstoreapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/androidmanagedstoreapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidmanagedstoreapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidmanagedstoreapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidmanagedstoreapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/androidmanagedstoreapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/androidmanagedstoreapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Add relationships by posting to the relationships collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|String|The Identity Name.|
|appStoreUrl|String|The Play for Work Store app URL.|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isPrivate|Boolean|Indicates whether the app is only available to a given enterprise's users.|
|isSystemApp|Boolean|Indicates whether the app is a preinstalled system app.|
|largeIcon|[mimeContent](../resources/intune-apps-mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|packageId|String|The package identifier.|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|supportsOemConfig|Boolean|Whether this app supports OEMConfig policy.|
|totalLicenseCount|Int32|The total number of VPP licenses.|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|usedLicenseCount|Int32|The number of VPP licenses in use.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|List of relationships for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreApp",
  "baseType": "microsoft.graph.mobileApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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

