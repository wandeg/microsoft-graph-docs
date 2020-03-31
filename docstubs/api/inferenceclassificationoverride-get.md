---
title: "Get inferenceClassificationOverride"
description: "Read properties and relationships of the inferenceClassificationOverride object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get inferenceClassificationOverride

Namespace: microsoft.graph

Read properties and relationships of the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.

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
GET /me/inferenceClassification/overrides/{inferenceClassificationOverrideId}
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
If successful, this method returns a `200 OK` response code and [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_inferenceclassificationoverride"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{inferenceClassificationOverrideId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "value": {
    "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
    "id": "48a3739e-739e-48a3-9e73-a3489e73a348",
    "classifyAs": "String",
    "senderEmailAddress": {
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "Name value",
      "address": "Address value"
    }
  }
}
```

