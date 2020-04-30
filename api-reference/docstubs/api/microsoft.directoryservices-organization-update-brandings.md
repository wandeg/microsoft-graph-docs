---
title: "Update brandings"
description: "Update the properties of a brandings object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update brandings

Namespace: Microsoft.DirectoryServices

Update the properties of a brandings object.

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
PATCH /organization/{organizationId}/brandings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object.

The following table shows the properties that are required when you create the [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|backgroundColor|String|**TODO: Add Description**|
|backgroundImage|Stream|**TODO: Add Description**|
|bannerLogo|Stream|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|signInPageText|String|**TODO: Add Description**|
|squareLogo|Stream|**TODO: Add Description**|
|usernameHintText|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_brandings"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/organization/{organizationId}/brandings
Content-Type: application/json
Content-length: 338

{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBranding",
  "backgroundColor": "Background Color value",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "Locale value",
  "signInPageText": "Sign In Page Text value",
  "squareLogo": "Stream",
  "usernameHintText": "Username Hint Text value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBranding",
  "id": "3f95260b-260b-3f95-0b26-953f0b26953f",
  "backgroundColor": "Background Color value",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "Locale value",
  "signInPageText": "Sign In Page Text value",
  "squareLogo": "Stream",
  "usernameHintText": "Username Hint Text value"
}
```

