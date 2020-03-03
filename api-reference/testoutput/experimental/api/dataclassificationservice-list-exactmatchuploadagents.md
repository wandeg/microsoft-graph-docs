---
title: "List exactMatchUploadAgents"
description: "Get the exactMatchUploadAgents from the exactMatchUploadAgents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List exactMatchUploadAgents

Namespace: microsoft.graph

Get the exactMatchUploadAgents from the exactMatchUploadAgents navigation property.

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
GET /dataClassification/exactMatchUploadAgents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchuploadagent"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/exactMatchUploadAgents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.exactmatchuploadagent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
      "id": "1721cbcf-cbcf-1721-cfcb-2117cfcb2117",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:02:11.4839005+03:00"
    }
  ]
}
```

