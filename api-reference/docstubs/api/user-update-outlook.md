---
title: "Update outlook"
description: "Update the properties of an outlook object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update outlook

Namespace: microsoft.graph

Update the properties of an outlook object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/outlook
PATCH /users/{usersId}/outlook
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [outlookUser](../resources/outlookuser.md) object.

The following table shows the properties that are required when you create the [outlookUser](../resources/outlookuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookUser](../resources/outlookuser.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_outlook"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/outlook
Content-Type: application/json
Content-length: 53

{
  "@odata.type": "#microsoft.graph.outlookUser"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.outlookUser",
  "id": "8f7daf30-af30-8f7d-30af-7d8f30af7d8f"
}
```

