---
title: "depEnrollmentProfile resource type"
description: "The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# depEnrollmentProfile resource type

The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.


Inherits from [enrollmentProfile](../resources/enrollmentProfile.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List depEnrollmentProfiles](../api/depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/depEnrollmentProfile.md) collection|List properties and relationships of the [depEnrollmentProfile](../resources/depenrollmentprofile.md) objects.|
|[Get depEnrollmentProfile](../api/depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/depEnrollmentProfile.md)|Read properties and relationships of the [depEnrollmentProfile](../resources/depenrollmentprofile.md) object.|
|[Create depEnrollmentProfile](../api/depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/depEnrollmentProfile.md)|Create a new [depEnrollmentProfile](../resources/depenrollmentprofile.md) object.|
|[Delete depEnrollmentProfile](../api/depenrollmentprofile-delete.md)|None|Deletes a [depEnrollmentProfile](../resources/depenrollmentprofile.md).|
|[Update depEnrollmentProfile](../api/depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/depEnrollmentProfile.md)|Update the properties of a [depEnrollmentProfile](../resources/depenrollmentprofile.md) object.|
|[setDefaultProfile](../api/depenrollmentprofile-setdefaultprofile.md)|None||
|[exportMobileConfig](../api/depenrollmentprofile-exportmobileconfig.md)|String||
|[updateDeviceProfileAssignment](../api/depenrollmentprofile-updatedeviceprofileassignment.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdDisabled|Boolean|Indicates if Apple id setup pane is disabled|
|applePayDisabled|Boolean|Indicates if Apple pay setup pane is disabled|
|awaitDeviceConfiguredConfirmation|Boolean|Indicates if the device will need to wait for configured confirmation|
|configurationEndpointUrl|String|Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|description|String|Description of the profile Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|diagnosticsDisabled|Boolean|Indicates if diagnostics setup pane is disabled|
|displayName|String|Name of the profile Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Indicates to authenticate with Apple Setup Assistant instead of Company Portal. Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|enableSharedIPad|Boolean|This indicates whether the device is to be enrolled in a mode which enables multi user scenarios. Only applicable in shared iPads.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|Indicates if this is the default profile|
|isMandatory|Boolean|Indicates if the profile is mandatory|
|iTunesPairingMode|Enumeration|Indicates the iTunes pairing mode. Possible values are: `disallow`, `allow`, `requiresCertificate`.|
|locationDisabled|Boolean|Indicates if Location service setup pane is disabled|
|macOSFileVaultDisabled|Boolean|Indicates if Mac OS file vault is disabled|
|macOSRegistrationDisabled|Boolean|Indicates if Mac OS registration is disabled|
|managementCertificates|[managementCertificateWithThumbprint](../resources/managementCertificateWithThumbprint.md) collection|Management certificates for Apple Configurator|
|passCodeDisabled|Boolean|Indicates if Passcode setup pane is disabled|
|profileRemovalDisabled|Boolean|Indicates if the profile removal option is disabled|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|requiresUserAuthentication|Boolean|Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|restoreBlocked|Boolean|Indicates if Restore setup pane is blocked|
|restoreFromAndroidDisabled|Boolean|Indicates if Restore from Android is disabled|
|sharedIPadMaximumUserCount|Int32|This specifies the maximum number of users that can use a shared iPad. Only applicable in shared iPad mode.|
|siriDisabled|Boolean|Indicates if siri setup pane is disabled|
|supervisedModeEnabled|Boolean|Supervised mode, True to enable, false otherwise. See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.|
|supportDepartment|String|Support department information|
|supportPhoneNumber|String|Support phone number|
|termsAndConditionsDisabled|Boolean|Indicates if 'Terms and Conditions' setup pane is disabled|
|touchIdDisabled|Boolean|Indicates if touch id setup pane is disabled|
|zoomDisabled|Boolean|Indicates if zoom setup pane is disabled|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile",
  "baseType": "microsoft.graph.enrollmentProfile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
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
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```

