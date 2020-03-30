---
title: "Update columnLink"
description: "Update the properties of a columnLink object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update columnLink

Namespace: microsoft.graph

Update the properties of a [columnLink](../resources/columnlink.md) object.

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
PATCH /me/joinedGroups/{groupId}/drive/list/contentTypes/{contentTypeId}/columnLinks/{columnLinkId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [columnLink](../resources/columnlink.md) object.

The following table shows the properties that are required when you create the [columnLink](../resources/columnlink.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [columnLink](../resources/columnlink.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_columnlink"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/list/contentTypes/{contentTypeId}/columnLinks/{columnLinkId}
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.columnLink",
  "name": "Name value"
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
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.columnLink",
  "id": "d60c1807-1807-d60c-0718-0cd607180cd6",
  "name": "Name value"
}
```

