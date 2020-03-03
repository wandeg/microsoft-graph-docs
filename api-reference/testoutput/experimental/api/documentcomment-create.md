---
title: "Create documentComment"
description: "Create a new documentComment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create documentComment

Namespace: microsoft.graph

Create a new [documentComment](../resources/documentcomment.md) object.

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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [documentComment](../resources/documentcomment.md) object.

The following table shows the properties that are required when you create the [documentComment](../resources/documentcomment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|String||



## Response
If successful, this method returns a `201 Created` response code and a [documentComment](../resources/documentcomment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_documentcomment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments
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
  "truncated": true,
  "@odata.type": "microsoft.graph.documentcomment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 137

{
  "@odata.type": "#microsoft.graph.documentComment",
  "id": "4c14e6cf-e6cf-4c14-cfe6-144ccfe6144c",
  "content": "Content value"
}
```

