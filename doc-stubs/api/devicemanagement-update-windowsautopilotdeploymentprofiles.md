---
title: "Update windowsAutopilotDeploymentProfiles"
description: "Update the properties of a windowsAutopilotDeploymentProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windowsAutopilotDeploymentProfiles

Namespace: microsoft.graph

Update the properties of a windowsAutopilotDeploymentProfiles object.

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
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.

The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|language|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/outofboxexperiencesettings.md)|**TODO: Add Description**|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/windowsenrollmentstatusscreensettings.md)|**TODO: Add Description**|
|extractHardwareHash|Boolean|**TODO: Add Description**|
|deviceNameTemplate|String|**TODO: Add Description**|
|deviceType|windowsAutopilotDeviceType|**TODO: Add Description**. Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.|
|enableWhiteGlove|Boolean|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windowsautopilotdeploymentprofiles"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-Type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
  },
  "extractHardwareHash": "Boolean",
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "bec4b8e0-b8e0-bec4-e0b8-c4bee0b8c4be",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
  },
  "extractHardwareHash": "Boolean",
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

