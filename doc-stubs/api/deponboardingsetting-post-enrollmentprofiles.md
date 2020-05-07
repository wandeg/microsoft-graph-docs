---
title: "Create enrollmentProfiles"
description: "Create a new enrollmentProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create enrollmentProfiles

Namespace: microsoft.graph

Create a new enrollmentProfiles object.

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [enrollmentProfile](../resources/enrollmentprofile.md) object.

The following table shows the properties that are required when you create the [enrollmentProfile](../resources/enrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|requiresUserAuthentication|Boolean|**TODO: Add Description**|
|configurationEndpointUrl|String|**TODO: Add Description**|
|enableAuthenticationViaCompanyPortal|Boolean|**TODO: Add Description**|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [enrollmentProfile](../resources/enrollmentprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_enrollmentprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-Type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": "Boolean",
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": "Boolean",
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.enrollmentprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "5d3f2459-2459-5d3f-5924-3f5d59243f5d",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": "Boolean",
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": "Boolean",
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean"
}
```

