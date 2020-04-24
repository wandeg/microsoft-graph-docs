---
title: "Get intuneBrandingProfile"
description: "Read the properties and relationships of an intuneBrandingProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get intuneBrandingProfile

Namespace: microsoft.graph

Read the properties and relationships of an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [intuneBrandingProfile](../resources/intunebrandingprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_intunebrandingprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfile",
    "id": "bcf270a6-70a6-bcf2-a670-f2bca670f2bc",
    "profileName": "Profile Name value",
    "profileDescription": "Profile Description value",
    "isDefaultProfile": true,
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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
    "showOfficeWebApps": true,
    "sendDeviceOwnershipChangePushNotification": true,
    "enrollmentAvailability": "String",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```

