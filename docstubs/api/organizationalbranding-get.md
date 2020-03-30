---
title: "Get organizationalBranding"
description: "Read properties and relationships of the organizationalBranding object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get organizationalBranding

Namespace: microsoft.graph

Read properties and relationships of the [organizationalBranding](../resources/organizationalbranding.md) object.

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
GET /organization/{organizationId}/brandings/{organizationalBrandingId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [organizationalBranding](../resources/organizationalbranding.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/brandings/{organizationalBrandingId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBranding"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 412

{
  "value": {
    "@odata.type": "#microsoft.graph.organizationalBranding",
    "id": "178d2588-2588-178d-8825-8d1788258d17",
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

