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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [rbacApplication](../resources/rbacapplication.md) object.

The following table shows the properties that are required when you create the [rbacApplication](../resources/rbacapplication.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [rbacApplication](../resources/rbacapplication.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_rbacapplication"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory
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
  "id": "ee5a1d67-1d67-ee5a-671d-5aee671d5aee"
}
```

