---
title: "List taskFolders"
description: "Get the outlookTaskFolders from the taskFolders navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List taskFolders

Namespace: microsoft.graph

Get the outlookTaskFolders from the taskFolders navigation property.

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
GET /me/outlook/taskFolders
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/outlook/taskFolders
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.outlooktaskfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookTaskFolder",
      "id": "4e07791c-791c-4e07-1c79-074e1c79074e",
      "changeKey": "Change Key value",
      "name": "Name value",
      "isDefaultFolder": true,
      "parentGroupKey": "fd4c385c-385c-fd4c-5c38-4cfd5c384cfd"
    }
  ]
}
```

