---
title: "Get documentComment"
description: "Read properties and relationships of the documentComment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get documentComment

Namespace: microsoft.graph

Read properties and relationships of the [documentComment](../resources/documentcomment.md) object.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}
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
If successful, this method returns a `200 OK` response code and [documentComment](../resources/documentcomment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_documentcomment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.documentComment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 162

{
  "value": {
    "@odata.type": "#microsoft.graph.documentComment",
    "id": "2a82ba7b-ba7b-2a82-7bba-822a7bba822a",
    "content": "Content value"
  }
}
```

