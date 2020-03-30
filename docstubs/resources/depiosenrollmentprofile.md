---
title: "depIOSEnrollmentProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# depIOSEnrollmentProfile resource type


Namespace: microsoft.graph




Inherits from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get depIOSEnrollmentProfile](../api/depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md)|Read properties and relationships of the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.|
|[Update depIOSEnrollmentProfile](../api/depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md)|Update the properties of a [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appearanceScreenDisabled|Boolean||
|appleIdDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|awaitDeviceConfiguredConfirmation|Boolean||
|companyPortalVppTokenId|String||
|configurationEndpointUrl|String| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|configurationWebUrl|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|description|String| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|deviceNameTemplate|String| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|deviceToDeviceMigrationDisabled|Boolean||
|diagnosticsDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|displayName|String| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|displayToneSetupDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|enableSharedIPad|Boolean||
|enableSingleAppEnrollmentMode|Boolean||
|expressLanguageScreenDisabled|Boolean||
|homeButtonScreenDisabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|iMessageAndFaceTimeScreenDisabled|Boolean||
|isDefault|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|isMandatory|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|iTunesPairingMode|Enumeration| Possible values are: `disallow`, `allow`, `requiresCertificate`.|
|locationDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|managementCertificates|[managementCertificateWithThumbprint](../resources/managementcertificatewiththumbprint.md) collection||
|onBoardingScreenDisabled|Boolean||
|passCodeDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|preferredLanguageScreenDisabled|Boolean||
|privacyPaneDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requiresUserAuthentication|Boolean| Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|restoreBlocked|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|restoreFromAndroidDisabled|Boolean||
|screenTimeScreenDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|sharedIPadMaximumUserCount|Int32||
|simSetupScreenDisabled|Boolean||
|siriDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|softwareUpdateScreenDisabled|Boolean||
|supervisedModeEnabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportDepartment|String| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportPhoneNumber|String| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|watchMigrationScreenDisabled|Boolean||
|welcomeScreenDisabled|Boolean||
|zoomDisabled|Boolean| Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
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

