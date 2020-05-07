---
title: "enrollmentProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# enrollmentProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[setDefaultProfile](../api/enrollmentprofile-setdefaultprofile.md)|None|**TODO: Add Description**|
|[exportMobileConfig](../api/enrollmentprofile-exportmobileconfig.md)|String|**TODO: Add Description**|
|[updateDeviceProfileAssignment](../api/enrollmentprofile-updatedeviceprofileassignment.md)|None|**TODO: Add Description**|
|[List enrollmentProfiles](../api/deponboardingsetting-list-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md) collection|Get the enrollmentProfiles from the enrollmentProfiles navigation property.|
|[Create enrollmentProfiles](../api/deponboardingsetting-post-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Create a new enrollmentProfiles object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationEndpointUrl|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|enableAuthenticationViaCompanyPortal|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|**TODO: Add Description**|
|requiresUserAuthentication|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "requiresUserAuthentication": "Boolean",
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": "Boolean",
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean"
}
```

