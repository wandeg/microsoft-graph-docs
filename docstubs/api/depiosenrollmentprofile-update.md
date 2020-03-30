---
title: "Update depIOSEnrollmentProfile"
description: "Update the properties of a depIOSEnrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update depIOSEnrollmentProfile

Namespace: microsoft.graph

Update the properties of a [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.

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
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.

The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|description|String| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requiresUserAuthentication|Boolean| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|configurationEndpointUrl|String| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|isDefault|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportDepartment|String| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|passCodeDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|isMandatory|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|locationDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportPhoneNumber|String| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|zoomDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|siriDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|deviceNameTemplate|String| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|configurationWebUrl|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|iTunesPairingMode|Enumeration| Possible values are: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/managementcertificatewiththumbprint.md) collection||
|restoreFromAndroidDisabled|Boolean||
|awaitDeviceConfiguredConfirmation|Boolean||
|sharedIPadMaximumUserCount|Int32||
|enableSharedIPad|Boolean||
|companyPortalVppTokenId|String||
|enableSingleAppEnrollmentMode|Boolean||
|homeButtonScreenDisabled|Boolean||
|iMessageAndFaceTimeScreenDisabled|Boolean||
|onBoardingScreenDisabled|Boolean||
|simSetupScreenDisabled|Boolean||
|softwareUpdateScreenDisabled|Boolean||
|watchMigrationScreenDisabled|Boolean||
|appearanceScreenDisabled|Boolean||
|expressLanguageScreenDisabled|Boolean||
|preferredLanguageScreenDisabled|Boolean||
|deviceToDeviceMigrationDisabled|Boolean||
|welcomeScreenDisabled|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_depiosenrollmentprofile"
}
-->
``` http

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
Content-Length: 2074

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "86049e1c-9e1c-8604-1c9e-04861c9e0486",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true
}
```

