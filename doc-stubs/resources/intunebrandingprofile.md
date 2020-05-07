---
title: "intuneBrandingProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# intuneBrandingProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/intunebrandingprofile-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/intunebrandingprofile-list-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|Get the intuneBrandingProfileAssignments from the assignments navigation property.|
|[Create assignments](../api/intunebrandingprofile-post-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intunebrandingprofile-delete-assignments.md)|None|Delete an [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|
|[Update assignments](../api/intunebrandingprofile-update-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Update the properties of an assignments object.|
|[Get intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Read the properties and relationships of an [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection|**TODO: Add Description**|
|contactITEmailAddress|String|**TODO: Add Description**|
|contactITName|String|**TODO: Add Description**|
|contactITNotes|String|**TODO: Add Description**|
|contactITPhoneNumber|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|customPrivacyMessage|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|enrollmentAvailability|enrollmentAvailabilityOptions|**TODO: Add Description**. Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefaultProfile|Boolean|**TODO: Add Description**|
|isFactoryResetDisabled|Boolean|**TODO: Add Description**|
|isRemoveDeviceDisabled|Boolean|**TODO: Add Description**|
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|onlineSupportSiteName|String|**TODO: Add Description**|
|onlineSupportSiteUrl|String|**TODO: Add Description**|
|privacyUrl|String|**TODO: Add Description**|
|profileDescription|String|**TODO: Add Description**|
|profileName|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|sendDeviceOwnershipChangePushNotification|Boolean|**TODO: Add Description**|
|showAzureADEnterpriseApps|Boolean|**TODO: Add Description**|
|showDisplayNameNextToLogo|Boolean|**TODO: Add Description**|
|showLogo|Boolean|**TODO: Add Description**|
|showOfficeWebApps|Boolean|**TODO: Add Description**|
|themeColor|[rgbColor](../resources/rgbcolor.md)|**TODO: Add Description**|
|themeColorLogo|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": "Boolean",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor"
  },
  "showLogo": "Boolean",
  "showDisplayNameNextToLogo": "Boolean",
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": "Boolean",
  "isFactoryResetDisabled": "Boolean",
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction"
    }
  ],
  "showAzureADEnterpriseApps": "Boolean",
  "showOfficeWebApps": "Boolean",
  "sendDeviceOwnershipChangePushNotification": "Boolean",
  "enrollmentAvailability": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

