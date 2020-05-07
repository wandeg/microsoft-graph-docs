---
title: "List intuneBrandingProfiles"
description: "Get the intuneBrandingProfiles from the intuneBrandingProfiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List intuneBrandingProfiles

Namespace: microsoft.graph

Get the intuneBrandingProfiles from the intuneBrandingProfiles navigation property.

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
GET /deviceManagement/intuneBrandingProfiles
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intunebrandingprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_intunebrandingprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.intunebrandingprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfile",
      "id": "761ec44d-c44d-761e-4dc4-1e764dc41e76",
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
  ]
}
```

