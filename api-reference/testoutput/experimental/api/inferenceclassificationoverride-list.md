---
title: "List inferenceClassificationOverrides"
description: "List properties and relationships of the inferenceClassificationOverride objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List inferenceClassificationOverrides

Namespace: microsoft.graph

List properties and relationships of the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects.

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
GET /me/inferenceClassification/overrides
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_inferenceclassificationoverride"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/inferenceClassification/overrides
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.inferenceclassificationoverride)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
      "id": "31d3d2ff-d2ff-31d3-ffd2-d331ffd2d331",
      "classifyAs": "String",
      "senderEmailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      }
    }
  ]
}
```

