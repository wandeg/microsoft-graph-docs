---
title: "List defaultIosEnrollmentProfile"
description: "Get the depIOSEnrollmentProfiles from the defaultIosEnrollmentProfile navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List defaultIosEnrollmentProfile

Namespace: microsoft.graph

Get the depIOSEnrollmentProfiles from the defaultIosEnrollmentProfile navigation property.

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
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
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

If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_depiosenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.depiosenrollmentprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
      "id": "cca9ce7c-ce7c-cca9-7cce-a9cc7ccea9cc",
      "displayName": "String",
      "description": "String",
      "requiresUserAuthentication": "Boolean",
      "configurationEndpointUrl": "String",
      "enableAuthenticationViaCompanyPortal": "Boolean",
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean",
      "isDefault": "Boolean",
      "supervisedModeEnabled": "Boolean",
      "supportDepartment": "String",
      "passCodeDisabled": "Boolean",
      "isMandatory": "Boolean",
      "locationDisabled": "Boolean",
      "supportPhoneNumber": "String",
      "profileRemovalDisabled": "Boolean",
      "restoreBlocked": "Boolean",
      "appleIdDisabled": "Boolean",
      "termsAndConditionsDisabled": "Boolean",
      "touchIdDisabled": "Boolean",
      "applePayDisabled": "Boolean",
      "zoomDisabled": "Boolean",
      "siriDisabled": "Boolean",
      "diagnosticsDisabled": "Boolean",
      "displayToneSetupDisabled": "Boolean",
      "privacyPaneDisabled": "Boolean",
      "screenTimeScreenDisabled": "Boolean",
      "deviceNameTemplate": "String",
      "configurationWebUrl": "Boolean",
      "iTunesPairingMode": "String",
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
        }
      ],
      "restoreFromAndroidDisabled": "Boolean",
      "awaitDeviceConfiguredConfirmation": "Boolean",
      "sharedIPadMaximumUserCount": "Integer",
      "enableSharedIPad": "Boolean",
      "companyPortalVppTokenId": "String",
      "enableSingleAppEnrollmentMode": "Boolean",
      "homeButtonScreenDisabled": "Boolean",
      "iMessageAndFaceTimeScreenDisabled": "Boolean",
      "onBoardingScreenDisabled": "Boolean",
      "simSetupScreenDisabled": "Boolean",
      "softwareUpdateScreenDisabled": "Boolean",
      "watchMigrationScreenDisabled": "Boolean",
      "appearanceScreenDisabled": "Boolean",
      "expressLanguageScreenDisabled": "Boolean",
      "preferredLanguageScreenDisabled": "Boolean",
      "deviceToDeviceMigrationDisabled": "Boolean",
      "welcomeScreenDisabled": "Boolean"
    }
  ]
}
```

