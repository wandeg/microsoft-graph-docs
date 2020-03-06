---
title: "depIOSEnrollmentProfile resource type"
description: "The DepIOSEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile specific to iOS configuration. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# depIOSEnrollmentProfile resource type


Namespace: microsoft.graph

The DepIOSEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile specific to iOS configuration. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.


Inherits from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get depIOSEnrollmentProfile](../api/depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md)|Read properties and relationships of the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.|
|[Update depIOSEnrollmentProfile](../api/depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md)|Update the properties of a [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appearanceScreenDisabled|Boolean|Indicates if Apperance screen is disabled|
|appleIdDisabled|Boolean|Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|awaitDeviceConfiguredConfirmation|Boolean|Indicates if the device will need to wait for configured confirmation|
|companyPortalVppTokenId|String|If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing. 'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.|
|configurationEndpointUrl|String|Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|configurationWebUrl|Boolean|URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|description|String|Description of the profile Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|deviceNameTemplate|String|Sets a literal or name pattern. Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|deviceToDeviceMigrationDisabled|Boolean|Indicates if Device To Device Migration is disabled|
|diagnosticsDisabled|Boolean|Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|displayName|String|Name of the profile Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|displayToneSetupDisabled|Boolean|Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Indicates to authenticate with Apple Setup Assistant instead of Company Portal. Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|enableSharedIPad|Boolean|This indicates whether the device is to be enrolled in a mode which enables multi user scenarios. Only applicable in shared iPads.|
|enableSingleAppEnrollmentMode|Boolean|Tells the device to enable single app mode and apply app-lock during enrollment. Default is false. 'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.|
|expressLanguageScreenDisabled|Boolean|Indicates if Express Language screen is disabled|
|homeButtonScreenDisabled|Boolean|Indicates if home button sensitivity screen is disabled|
|id|String| Inherited from [entity](../resources/entity.md)|
|iMessageAndFaceTimeScreenDisabled|Boolean|Indicates if iMessage and FaceTime screen is disabled|
|isDefault|Boolean|Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|isMandatory|Boolean|Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|iTunesPairingMode|Enumeration|Indicates the iTunes pairing mode. Possible values are: `disallow`, `allow`, `requiresCertificate`.|
|locationDisabled|Boolean|Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|managementCertificates|[managementCertificateWithThumbprint](../resources/managementcertificatewiththumbprint.md) collection|Management certificates for Apple Configurator|
|onBoardingScreenDisabled|Boolean|Indicates if onboarding setup screen is disabled|
|passCodeDisabled|Boolean|Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|preferredLanguageScreenDisabled|Boolean|Indicates if Preferred language screen is disabled|
|privacyPaneDisabled|Boolean|Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|restoreBlocked|Boolean|Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|restoreFromAndroidDisabled|Boolean|Indicates if Restore from Android is disabled|
|screenTimeScreenDisabled|Boolean|Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|sharedIPadMaximumUserCount|Int32|This specifies the maximum number of users that can use a shared iPad. Only applicable in shared iPad mode.|
|simSetupScreenDisabled|Boolean|Indicates if the SIMSetup screen is disabled|
|siriDisabled|Boolean|Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|softwareUpdateScreenDisabled|Boolean|Indicates if the mandatory sofware update screen is disabled|
|supervisedModeEnabled|Boolean|Supervised mode, True to enable, false otherwise. See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information. Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportDepartment|String|Support department information Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|Support phone number Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|watchMigrationScreenDisabled|Boolean|Indicates if the watch migration screen is disabled|
|welcomeScreenDisabled|Boolean|Indicates if Weclome screen is disabled|
|zoomDisabled|Boolean|Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|

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

