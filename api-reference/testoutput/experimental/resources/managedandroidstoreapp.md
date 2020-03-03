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
|[List categories](../api/managedandroidstoreapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/managedandroidstoreapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/managedandroidstoreapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/managedandroidstoreapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/managedandroidstoreapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/managedandroidstoreapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/managedandroidstoreapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/managedandroidstoreapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/managedandroidstoreapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/managedandroidstoreapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Add relationships by posting to the relationships collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAvailability|Enumeration|The Application's availability. Inherited from [managedApp](../resources/managedapp.md). Possible values are: `global`, `lineOfBusiness`.|
|appStoreUrl|String|The Android AppStoreUrl.|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|The value for the minimum supported operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|packageId|String|The app's package ID.|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|version|String|The Application's version. Inherited from [managedApp](../resources/managedapp.md)|

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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
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
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

