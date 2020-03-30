---
title: "intuneBrandingProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# intuneBrandingProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get intuneBrandingProfile](../api/intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Read properties and relationships of the [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[Update intuneBrandingProfile](../api/intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intunebrandingprofile.md)|Update the properties of a [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.|
|[assign](../api/intunebrandingprofile-assign.md)|None||
|[List assignments](../api/intunebrandingprofile-list-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|Get the intuneBrandingProfileAssignments from the assignments navigation property.|
|[Add assignments](../api/intunebrandingprofile-post-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection||
|contactITEmailAddress|String||
|contactITName|String||
|contactITNotes|String||
|contactITPhoneNumber|String||
|createdDateTime|DateTimeOffset||
|customPrivacyMessage|String||
|displayName|String||
|enrollmentAvailability|Enumeration| Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefaultProfile|Boolean||
|isFactoryResetDisabled|Boolean||
|isRemoveDeviceDisabled|Boolean||
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)||
|lastModifiedDateTime|DateTimeOffset||
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)||
|onlineSupportSiteName|String||
|onlineSupportSiteUrl|String||
|privacyUrl|String||
|profileDescription|String||
|profileName|String||
|roleScopeTagIds|String collection||
|sendDeviceOwnershipChangePushNotification|Boolean||
|showAzureADEnterpriseApps|Boolean||
|showDisplayNameNextToLogo|Boolean||
|showLogo|Boolean||
|showOfficeWebApps|Boolean||
|themeColor|[rgbColor](../resources/rgbcolor.md)||
|themeColorLogo|[mimeContent](../resources/mimecontent.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
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
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

