---
title: "enrollmentProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enrollmentProfile resource type


Namespace: microsoft.graph




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
|configurationEndpointUrl|String||
|description|String||
|displayName|String||
|enableAuthenticationViaCompanyPortal|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean||
|requiresUserAuthentication|Boolean||

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

