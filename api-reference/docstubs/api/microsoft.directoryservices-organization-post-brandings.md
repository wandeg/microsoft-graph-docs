---
title: "Create brandings"
description: "Create a new brandings object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create brandings

Namespace: Microsoft.DirectoryServices

Create a new brandings object.

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
POST /organization/{organizationId}/brandings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and an [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_organizationalbranding_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/organization/{organizationId}/brandings
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
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.organizationalbranding"
}
-->
``` http
HTTP/1.1 201 Created
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

