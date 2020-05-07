---
title: "Add defaultIosEnrollmentProfile"
description: "Add defaultIosEnrollmentProfile by posting to the defaultIosEnrollmentProfile collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add defaultIosEnrollmentProfile

Namespace: microsoft.graph

Add defaultIosEnrollmentProfile by posting to the defaultIosEnrollmentProfile collection.

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.

The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|description|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|configurationEndpointUrl|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|isDefault|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportDepartment|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|passCodeDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|isMandatory|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|zoomDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|siriDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|deviceNameTemplate|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|configurationWebUrl|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|iTunesPairingMode|iTunesPairingMode|**TODO: Add Description**. Possible values are: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/managementcertificatewiththumbprint.md) collection|**TODO: Add Description**|
|restoreFromAndroidDisabled|Boolean|**TODO: Add Description**|
|awaitDeviceConfiguredConfirmation|Boolean|**TODO: Add Description**|
|sharedIPadMaximumUserCount|Int32|**TODO: Add Description**|
|enableSharedIPad|Boolean|**TODO: Add Description**|
|companyPortalVppTokenId|String|**TODO: Add Description**|
|enableSingleAppEnrollmentMode|Boolean|**TODO: Add Description**|
|homeButtonScreenDisabled|Boolean|**TODO: Add Description**|
|iMessageAndFaceTimeScreenDisabled|Boolean|**TODO: Add Description**|
|onBoardingScreenDisabled|Boolean|**TODO: Add Description**|
|simSetupScreenDisabled|Boolean|**TODO: Add Description**|
|softwareUpdateScreenDisabled|Boolean|**TODO: Add Description**|
|watchMigrationScreenDisabled|Boolean|**TODO: Add Description**|
|appearanceScreenDisabled|Boolean|**TODO: Add Description**|
|expressLanguageScreenDisabled|Boolean|**TODO: Add Description**|
|preferredLanguageScreenDisabled|Boolean|**TODO: Add Description**|
|deviceToDeviceMigrationDisabled|Boolean|**TODO: Add Description**|
|welcomeScreenDisabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_depiosenrollmentprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile/$ref
Content-Type: application/json
Content-length: 1981

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.depiosenrollmentprofile"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
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
```

