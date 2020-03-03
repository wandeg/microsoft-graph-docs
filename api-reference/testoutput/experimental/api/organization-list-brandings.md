---
title: "List brandings"
description: "Get the organizationalBrandings from the brandings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List brandings

Get the organizationalBrandings from the brandings navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}/brandings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [organizationalBranding](../resources/organizationalbranding.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/organization/{organizationId}/brandings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.organizationalbranding)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 444

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organizationalBranding",
      "id": "74e73f7b-3f7b-74e7-7b3f-e7747b3fe774",
      "backgroundColor": "Background Color value",
      "backgroundImage": "Stream",
      "bannerLogo": "Stream",
      "locale": "Locale value",
      "signInPageText": "Sign In Page Text value",
      "squareLogo": "Stream",
      "usernameHintText": "Username Hint Text value"
    }
  ]
}
```

