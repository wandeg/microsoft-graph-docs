---
title: "enrollmentProfile resource type"
description: "The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged. Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enrollmentProfile resource type


Namespace: microsoft.graph

The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged. Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get enrollmentProfile](../api/enrollmentprofile-get.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Read properties and relationships of the [enrollmentProfile](../resources/enrollmentprofile.md) object.|
|[Update enrollmentProfile](../api/enrollmentprofile-update.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Update the properties of a [enrollmentProfile](../resources/enrollmentprofile.md) object.|
|[setDefaultProfile](../api/enrollmentprofile-setdefaultprofile.md)|None||
|[exportMobileConfig](../api/enrollmentprofile-exportmobileconfig.md)|String||
|[updateDeviceProfileAssignment](../api/enrollmentprofile-updatedeviceprofileassignment.md)|None||
|[List enrollmentProfiles](../api/deponboardingsetting-list-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md) collection|Get the enrollmentProfiles from the enrollmentProfiles navigation property.|
|[Add enrollmentProfiles](../api/deponboardingsetting-post-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Add enrollmentProfiles by posting to the enrollmentProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationEndpointUrl|String|Configuration endpoint url to use for Enrollment|
|description|String|Description of the profile|
|displayName|String|Name of the profile|
|enableAuthenticationViaCompanyPortal|Boolean|Indicates to authenticate with Apple Setup Assistant instead of Company Portal.|
|id|String| Inherited from [entity](../resources/entity.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indicates that Company Portal is required on setup assistant enrolled devices|
|requiresUserAuthentication|Boolean|Indicates if the profile requires user authentication|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

