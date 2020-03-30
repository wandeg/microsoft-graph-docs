---
title: "Update enrollmentProfile"
description: "Update the properties of a enrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update enrollmentProfile

Namespace: microsoft.graph

Update the properties of a [enrollmentProfile](../resources/enrollmentprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [enrollmentProfile](../resources/enrollmentprofile.md) object.

The following table shows the properties that are required when you create the [enrollmentProfile](../resources/enrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|requiresUserAuthentication|Boolean||
|configurationEndpointUrl|String||
|enableAuthenticationViaCompanyPortal|Boolean||
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/enrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_enrollmentprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "8627d78b-d78b-8627-8bd7-27868bd72786",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

