---
title: "Update rbacApplication"
description: "Update the properties of a rbacApplication object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update rbacApplication

Namespace: microsoft.graph

Update the properties of a [rbacApplication](../resources/rbacapplication.md) object.

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
PATCH /roleManagement/directory
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [rbacApplication](../resources/rbacapplication.md) object.

The following table shows the properties that are required when you create the [rbacApplication](../resources/rbacapplication.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [rbacApplication](../resources/rbacapplication.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_rbacapplication"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/roleManagement/directory
Content-type: application/json
Content-length: 57

{
  "@odata.type": "#microsoft.graph.rbacApplication"
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
Content-Length: 106

{
  "@odata.type": "#microsoft.graph.rbacApplication",
  "id": "9bb972e4-72e4-9bb9-e472-b99be472b99b"
}
```

