---
title: "Create privilegedRole"
description: "Create a new privilegedRole object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedRole

Namespace: microsoft.graph

Create a new [privilegedRole](../resources/privilegedrole.md) object.

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
POST /privilegedRoles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedRole](../resources/privilegedrole.md) object.

The following table shows the properties that are required when you create the [privilegedRole](../resources/privilegedrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `201 Created` response code and a [privilegedRole](../resources/privilegedrole.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedrole_from_privilegedroles"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoles
Content-type: application/json
Content-length: 81

{
  "@odata.type": "#microsoft.graph.privilegedRole",
  "name": "Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedrole"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 130

{
  "@odata.type": "#microsoft.graph.privilegedRole",
  "id": "25742efb-2efb-2574-fb2e-7425fb2e7425",
  "name": "Name value"
}
```

