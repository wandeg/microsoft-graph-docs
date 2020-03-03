---
title: "microsoftStoreForBusinessApp resource type"
description: "Microsoft Store for Business Apps. This class does not support Create, Delete, or Update."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# microsoftStoreForBusinessApp resource type


Namespace: microsoft.graph

Microsoft Store for Business Apps. This class does not support Create, Delete, or Update.


Inherits from [mobileApp](../resources/mobileapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List microsoftStoreForBusinessApps](../api/microsoftstoreforbusinessapp-list.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) collection|List properties and relationships of the [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) objects.|
|[Get microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-get.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md)|Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) object.|
|[Create microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-create.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md)|Create a new [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) object.|
|[Delete microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-delete.md)|None|Deletes a [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md).|
|[Update microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-update.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md)|Update the properties of a [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) object.|
|[assign](../api/microsoftstoreforbusinessapp-assign.md)|None||
|[updateRelationships](../api/microsoftstoreforbusinessapp-updaterelationships.md)|None||
|[getRelatedAppStates](../api/microsoftstoreforbusinessapp-getrelatedappstates.md)|[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection||
|[List categories](../api/microsoftstoreforbusinessapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/microsoftstoreforbusinessapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/microsoftstoreforbusinessapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/microsoftstoreforbusinessapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/microsoftstoreforbusinessapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/microsoftstoreforbusinessapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/microsoftstoreforbusinessapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/microsoftstoreforbusinessapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/microsoftstoreforbusinessapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/microsoftstoreforbusinessapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Add relationships by posting to the relationships collection.|
|[List containedApps](../api/microsoftstoreforbusinessapp-list-containedapps.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection|Get the mobileContainedApps from the containedApps navigation property.|
|[Add containedApps](../api/microsoftstoreforbusinessapp-post-containedapps.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Add containedApps by posting to the containedApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
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
|licenseType|Enumeration|The app license type. Possible values are: `offline`, `online`.|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|The supported License Type.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|packageIdentityName|String|The app package identifier|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|productKey|String|The app product key|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|totalLicenseCount|Int32|The total number of Microsoft Store for Business licenses.|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|usedLicenseCount|Int32|The number of Microsoft Store for Business licenses in use.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection|The collection of contained apps in a mobileApp acting as a package.|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|List of relationships for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp",
  "baseType": "microsoft.graph.mobileApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

