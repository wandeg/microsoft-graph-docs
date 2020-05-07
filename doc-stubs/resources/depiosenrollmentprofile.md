---
title: "depIOSEnrollmentProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# depIOSEnrollmentProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appearanceScreenDisabled|Boolean|**TODO: Add Description**|
|appleIdDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|awaitDeviceConfiguredConfirmation|Boolean|**TODO: Add Description**|
|companyPortalVppTokenId|String|**TODO: Add Description**|
|configurationEndpointUrl|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|configurationWebUrl|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|description|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|deviceNameTemplate|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|deviceToDeviceMigrationDisabled|Boolean|**TODO: Add Description**|
|diagnosticsDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|displayName|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|displayToneSetupDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|enableSharedIPad|Boolean|**TODO: Add Description**|
|enableSingleAppEnrollmentMode|Boolean|**TODO: Add Description**|
|expressLanguageScreenDisabled|Boolean|**TODO: Add Description**|
|homeButtonScreenDisabled|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|iMessageAndFaceTimeScreenDisabled|Boolean|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|isMandatory|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|iTunesPairingMode|iTunesPairingMode|**TODO: Add Description**. Possible values are: `disallow`, `allow`, `requiresCertificate`.|
|locationDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|managementCertificates|[managementCertificateWithThumbprint](../resources/managementcertificatewiththumbprint.md) collection|**TODO: Add Description**|
|onBoardingScreenDisabled|Boolean|**TODO: Add Description**|
|passCodeDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|preferredLanguageScreenDisabled|Boolean|**TODO: Add Description**|
|privacyPaneDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|restoreBlocked|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|restoreFromAndroidDisabled|Boolean|**TODO: Add Description**|
|screenTimeScreenDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|sharedIPadMaximumUserCount|Int32|**TODO: Add Description**|
|simSetupScreenDisabled|Boolean|**TODO: Add Description**|
|siriDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|softwareUpdateScreenDisabled|Boolean|**TODO: Add Description**|
|supervisedModeEnabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportDepartment|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|watchMigrationScreenDisabled|Boolean|**TODO: Add Description**|
|welcomeScreenDisabled|Boolean|**TODO: Add Description**|
|zoomDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile",
  "baseType": "microsoft.graph.depEnrollmentBaseProfile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "String (identifier)",
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

