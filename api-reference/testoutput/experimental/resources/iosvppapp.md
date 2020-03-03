---
title: "iosVppApp resource type"
description: "Contains properties and inherited properties for iOS Volume-Purchased Program (VPP) Apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosVppApp resource type

Contains properties and inherited properties for iOS Volume-Purchased Program (VPP) Apps.


Inherits from [mobileApp](../resources/mobileApp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppApps](../api/iosvppapp-list.md)|[iosVppApp](../resources/iosVppApp.md) collection|List properties and relationships of the [iosVppApp](../resources/iosvppapp.md) objects.|
|[Get iosVppApp](../api/iosvppapp-get.md)|[iosVppApp](../resources/iosVppApp.md)|Read properties and relationships of the [iosVppApp](../resources/iosvppapp.md) object.|
|[Create iosVppApp](../api/iosvppapp-create.md)|[iosVppApp](../resources/iosVppApp.md)|Create a new [iosVppApp](../resources/iosvppapp.md) object.|
|[Delete iosVppApp](../api/iosvppapp-delete.md)|None|Deletes a [iosVppApp](../resources/iosvppapp.md).|
|[Update iosVppApp](../api/iosvppapp-update.md)|[iosVppApp](../resources/iosVppApp.md)|Update the properties of a [iosVppApp](../resources/iosvppapp.md) object.|
|[assign](../api/iosvppapp-assign.md)|None||
|[updateRelationships](../api/iosvppapp-updaterelationships.md)|None||
|[getRelatedAppStates](../api/iosvppapp-getrelatedappstates.md)|[mobileAppRelationshipState](../resources/intune-apps-mobileAppRelationshipState.md) collection||
|[revokeAllLicenses](../api/iosvppapp-revokealllicenses.md)|None||
|[revokeUserLicense](../api/iosvppapp-revokeuserlicense.md)|None||
|[revokeDeviceLicense](../api/iosvppapp-revokedevicelicense.md)|None||
|[List categories](../api/iosvppapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/iosvppapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/iosvppapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/iosvppapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/iosvppapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/iosvppapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/iosvppapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/iosvppapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/iosvppapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/iosvppapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md)|Add relationships by posting to the relationships collection.|
|[List assignedLicenses](../api/iosvppapp-list-assignedlicenses.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md) collection|Get the iosVppAppAssignedLicenses from the assignedLicenses navigation property.|
|[Add assignedLicenses](../api/iosvppapp-post-assignedlicenses.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md)|Add assignedLicenses by posting to the assignedLicenses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosDeviceType.md)|The applicable iOS Device Type.|
|appStoreUrl|String|The store URL.|
|bundleId|String|The Identity Name.|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|largeIcon|[mimeContent](../resources/intune-apps-mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|licensingType|[vppLicensingType](../resources/intune-apps-vppLicensingType.md)|The supported License Type.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md). Possible values are: `notPublished`, `processing`, `published`.|
|releaseDateTime|DateTimeOffset|The VPP application release date and time.|
|revokeLicenseActionResults|[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosVppAppRevokeLicensesActionResult.md) collection|Results of revoke license actions on this app.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|totalLicenseCount|Int32|The total number of VPP licenses.|
|uploadState|Int32|The upload state. Inherited from [mobileApp](../resources/intune-apps-mobileApp.md)|
|usedLicenseCount|Int32|The number of VPP licenses in use.|
|vppTokenAccountType|Enumeration|The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. Possible values are: `business`, `education`. Possible values are: `business`, `education`.|
|vppTokenAppleId|String|The Apple Id associated with the given Apple Volume Purchase Program Token.|
|vppTokenId|String|Identifier of the VPP token associated with this app.|
|vppTokenOrganizationName|String|The organization associated with the Apple Volume Purchase Program Token|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignedLicenses|[iosVppAppAssignedLicense](../resources/intune-apps-iosVppAppAssignedLicense.md) collection|The licenses assigned to this app.|
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
  "@odata.type": "microsoft.graph.iosVppApp",
  "baseType": "microsoft.graph.mobileApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "releaseDateTime": "String (timestamp)",
  "appStoreUrl": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "String",
  "vppTokenAccountType": "String",
  "vppTokenAppleId": "String",
  "bundleId": "String",
  "vppTokenId": "String",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "managedDeviceId": "String",
      "totalLicensesCount": 1024,
      "failedLicensesCount": 1024,
      "actionFailureReason": "String",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ]
}
```

