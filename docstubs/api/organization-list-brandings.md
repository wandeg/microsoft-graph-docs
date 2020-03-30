---
title: "List brandings"
description: "Get the organizationalBrandings from the brandings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List brandings

Namespace: microsoft.graph

Get the organizationalBrandings from the brandings navigation property.

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
GET /organization/{organizationId}/brandings
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
If successful, this method returns a `200 OK` response code and a collection of [organizationalBranding](../resources/organizationalbranding.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_organizationalbranding"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/brandings
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
      "id": "58a80641-0641-58a8-4106-a8584106a858",
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

