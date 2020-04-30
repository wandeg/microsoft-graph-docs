---
title: "Get organizationalBranding"
description: "Read properties and relationships of an organizationalBranding object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get organizationalBranding

Namespace: Microsoft.DirectoryServices

Read properties and relationships of an [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object.

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
GET /organization/{organizationId}/brandings/{organizationalBrandingId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}
-->
``` http
GET https://graph.microsoft.com/changelog/organization/{organizationId}/brandings/{organizationalBrandingId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.organizationalBranding"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

