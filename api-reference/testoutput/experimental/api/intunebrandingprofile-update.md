---
title: "Update intuneBrandingProfile"
description: "Update the properties of a intuneBrandingProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update intuneBrandingProfile

Namespace: microsoft.graph

Update the properties of a [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.

The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intunebrandingprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|profileName|String|Name of the profile|
|profileDescription|String|Description of the profile|
|isDefaultProfile|Boolean|Boolean that represents whether the profile is used as default or not|
|createdDateTime|DateTimeOffset|Time when the BrandingProfile was created|
|lastModifiedDateTime|DateTimeOffset|Time when the BrandingProfile was last modified|
|displayName|String|Company/organization name that is displayed to end users|
|themeColor|[rgbColor](../resources/rgbcolor.md)|Primary theme color used in the Company Portal applications and web portal|
|showLogo|Boolean|Boolean that represents whether the administrator-supplied logo images are shown or not|
|showDisplayNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not|
|themeColorLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a theme color background behind the logo|
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a light background behind the logo|
|landingPageCustomizedImage|[mimeContent](../resources/mimecontent.md)|Customized image displayed in Company Portal apps landing page|
|contactITName|String|Name of the person/organization responsible for IT support|
|contactITPhoneNumber|String|Phone number of the person/organization responsible for IT support|
|contactITEmailAddress|String|E-mail address of the person/organization responsible for IT support|
|contactITNotes|String|Text comments regarding the person/organization responsible for IT support|
|onlineSupportSiteUrl|String|URL to the company/organization’s IT helpdesk site|
|onlineSupportSiteName|String|Display name of the company/organization’s IT helpdesk site|
|privacyUrl|String|URL to the company/organization’s privacy policy|
|customPrivacyMessage|String|Text comments regarding what the admin has access to on the device|
|isRemoveDeviceDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.|
|isFactoryResetDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/companyportalblockedaction.md) collection|Collection of blocked actions on the company portal as per platform and device ownership types.|
|showAzureADEnterpriseApps|Boolean|Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal|
|showOfficeWebApps|Boolean|Boolean that indicates if Office WebApps will be shown in Company Portal|



## Response
If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intunebrandingprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_intunebrandingprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1505

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
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
  "showOfficeWebApps": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1677

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "bb0219c2-19c2-bb02-c219-02bbc21902bb",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
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
  "showOfficeWebApps": true
}
```

