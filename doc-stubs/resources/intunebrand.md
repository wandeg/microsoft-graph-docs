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
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection|**TODO: Add Description**|
|contactITEmailAddress|String|**TODO: Add Description**|
|contactITName|String|**TODO: Add Description**|
|contactITNotes|String|**TODO: Add Description**|
|contactITPhoneNumber|String|**TODO: Add Description**|
|customPrivacyMessage|String|**TODO: Add Description**|
|darkBackgroundLogo|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|enrollmentAvailability|enrollmentAvailabilityOptions|**TODO: Add Description**. Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|isFactoryResetDisabled|Boolean|**TODO: Add Description**|
|isRemoveDeviceDisabled|Boolean|**TODO: Add Description**|
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|onlineSupportSiteName|String|**TODO: Add Description**|
|onlineSupportSiteUrl|String|**TODO: Add Description**|
|privacyUrl|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|sendDeviceOwnershipChangePushNotification|Boolean|**TODO: Add Description**|
|showAzureADEnterpriseApps|Boolean|**TODO: Add Description**|
|showDisplayNameNextToLogo|Boolean|**TODO: Add Description**|
|showLogo|Boolean|**TODO: Add Description**|
|showNameNextToLogo|Boolean|**TODO: Add Description**|
|showOfficeWebApps|Boolean|**TODO: Add Description**|
|themeColor|[rgbColor](../resources/rgbcolor.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.rgbColor"
  },
  "showLogo": "Boolean",
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "showNameNextToLogo": "Boolean",
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "showDisplayNameNextToLogo": "Boolean",
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
  "enrollmentAvailability": "String"
}
```

