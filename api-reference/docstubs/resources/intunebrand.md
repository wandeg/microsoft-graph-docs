---
title: "intuneBrand resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# intuneBrand resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection|Collection of blocked actions on the company portal as per platform and device ownership types.|
|contactITEmailAddress|String|Email address of the person/organization responsible for IT support.|
|contactITName|String|Name of the person/organization responsible for IT support.|
|contactITNotes|String|Text comments regarding the person/organization responsible for IT support.|
|contactITPhoneNumber|String|Phone number of the person/organization responsible for IT support.|
|customPrivacyMessage|String|Custom privacy message.|
|darkBackgroundLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a dark background behind the logo.|
|displayName|String|Company/organization name that is displayed to end users.|
|enrollmentAvailability|enrollmentAvailabilityOptions|Customized device enrollment flow displayed to the end user . Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|isFactoryResetDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.|
|isRemoveDeviceDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.|
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)|Customized image displayed in Company Portal app landing page|
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a light background behind the logo.|
|onlineSupportSiteName|String|Display name of the company/organization’s IT helpdesk site.|
|onlineSupportSiteUrl|String|URL to the company/organization’s IT helpdesk site.|
|privacyUrl|String|URL to the company/organization’s privacy policy.|
|roleScopeTagIds|String collection|List of scope tags assigned to the default branding profile|
|sendDeviceOwnershipChangePushNotification|Boolean|Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate|
|showAzureADEnterpriseApps|Boolean|Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal|
|showDisplayNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.|
|showLogo|Boolean|Boolean that represents whether the administrator-supplied logo images are shown or not shown.|
|showNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.|
|showOfficeWebApps|Boolean|Boolean that indicates if Office WebApps will be shown in Company Portal|
|themeColor|[rgbColor](../resources/rgbcolor.md)|Primary theme color used in the Company Portal applications and web portal.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
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
  "enrollmentAvailability": "String"
}
```

