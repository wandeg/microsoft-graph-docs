---
title: "List mentions"
description: "Get the mentions from the mentions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mentions

Namespace: microsoft.graph

Get the mentions from the mentions navigation property.

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
GET /me/messages/{messageId}/mentions
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
If successful, this method returns a `200 OK` response code and a collection of [mention](../resources/mention.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mention"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/mentions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mention)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mention",
      "id": "f8b34e55-4e55-f8b3-554e-b3f8554eb3f8",
      "mentioned": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      },
      "mentionText": "Mention Text value",
      "clientReference": "Client Reference value",
      "createdBy": {
        "@odata.type": "microsoft.graph.emailAddress"
      },
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "serverCreatedDateTime": "2016-12-31T23:59:11.6731698+03:00",
      "deepLink": "Deep Link value",
      "application": "Application value"
    }
  ]
}
```

