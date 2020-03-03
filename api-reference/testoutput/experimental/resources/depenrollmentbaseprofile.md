---
title: "depEnrollmentBaseProfile resource type"
description: "The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# depEnrollmentBaseProfile resource type

The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.


Inherits from [enrollmentProfile](../resources/enrollmentProfile.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List depEnrollmentBaseProfiles](../api/depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/depEnrollmentBaseProfile.md) collection|List properties and relationships of the [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md) objects.|
|[Get depEnrollmentBaseProfile](../api/depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/depEnrollmentBaseProfile.md)|Read properties and relationships of the [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md) object.|
|[setDefaultProfile](../api/depenrollmentbaseprofile-setdefaultprofile.md)|None||
|[exportMobileConfig](../api/depenrollmentbaseprofile-exportmobileconfig.md)|String||
|[updateDeviceProfileAssignment](../api/depenrollmentbaseprofile-updatedeviceprofileassignment.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdDisabled|Boolean|Indicates if Apple id setup pane is disabled|
|applePayDisabled|Boolean|Indicates if Apple pay setup pane is disabled|
|configurationEndpointUrl|String|Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|configurationWebUrl|Boolean|URL for setup assistant login|
|description|String|Description of the profile Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|deviceNameTemplate|String|Sets a literal or name pattern.|
|diagnosticsDisabled|Boolean|Indicates if diagnostics setup pane is disabled|
|displayName|String|Name of the profile Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|displayToneSetupDisabled|Boolean|Indicates if displaytone setup screen is disabled|
|enableAuthenticationViaCompanyPortal|Boolean|Indicates to authenticate with Apple Setup Assistant instead of Company Portal. Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|Indicates if this is the default profile|
|isMandatory|Boolean|Indicates if the profile is mandatory|
|locationDisabled|Boolean|Indicates if Location service setup pane is disabled|
|passCodeDisabled|Boolean|Indicates if Passcode setup pane is disabled|
|privacyPaneDisabled|Boolean|Indicates if privacy screen is disabled|
|profileRemovalDisabled|Boolean|Indicates if the profile removal option is disabled|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|requiresUserAuthentication|Boolean|Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/enrollmentProfile.md)|
|restoreBlocked|Boolean|Indicates if Restore setup pane is blocked|
|screenTimeScreenDisabled|Boolean|Indicates if screen timeout setup is disabled|
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
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile",
  "baseType": "microsoft.graph.enrollmentProfile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
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
  "configurationWebUrl": true
}
```

