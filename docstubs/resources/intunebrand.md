---
title: "intuneBrand resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# intuneBrand resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection||
|contactITEmailAddress|String||
|contactITName|String||
|contactITNotes|String||
|contactITPhoneNumber|String||
|customPrivacyMessage|String||
|darkBackgroundLogo|[mimeContent](../resources/mimecontent.md)||
|displayName|String||
|enrollmentAvailability|Enumeration| Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|isFactoryResetDisabled|Boolean||
|isRemoveDeviceDisabled|Boolean||
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)||
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)||
|onlineSupportSiteName|String||
|onlineSupportSiteUrl|String||
|privacyUrl|String||
|roleScopeTagIds|String collection||
|sendDeviceOwnershipChangePushNotification|Boolean||
|showAzureADEnterpriseApps|Boolean||
|showDisplayNameNextToLogo|Boolean||
|showLogo|Boolean||
|showNameNextToLogo|Boolean||
|showOfficeWebApps|Boolean||
|themeColor|[rgbColor](../resources/rgbcolor.md)||

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

