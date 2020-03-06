---
title: "Update documentComment"
description: "Update the properties of a documentComment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update documentComment

Namespace: microsoft.graph

Update the properties of a [documentComment](../resources/documentcomment.md) object.

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
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [documentComment](../resources/documentcomment.md) object.

The following table shows the properties that are required when you create the [documentComment](../resources/documentcomment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [documentComment](../resources/documentcomment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_documentcomment"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}
Content-type: application/json
Content-length: 88

{
  "@odata.type": "#microsoft.graph.documentComment",
  "content": "Content value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 137

{
  "@odata.type": "#microsoft.graph.documentComment",
  "id": "2a82ba7b-ba7b-2a82-7bba-822a7bba822a",
  "content": "Content value"
}
```

