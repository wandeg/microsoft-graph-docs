---
title: "Update appScope"
description: "Update the properties of a appScope object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update appScope

Namespace: microsoft.graph

Update the properties of a [appScope](../resources/appscope.md) object.

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
PATCH /roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}/appScope
PATCH /roleManagement/deviceManagement/roleAssignments/{unifiedRoleAssignmentMultipleId}/appScopes/{appScopeId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [appScope](../resources/appscope.md) object.

The following table shows the properties that are required when you create the [appScope](../resources/appscope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [appScope](../resources/appscope.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_appscope"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}/appScope
Content-type: application/json
Content-length: 115

{
  "@odata.type": "#microsoft.graph.appScope",
  "type": "Type value",
  "displayName": "Display Name value"
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
Content-Length: 164

{
  "@odata.type": "#microsoft.graph.appScope",
  "id": "d658835a-835a-d658-5a83-58d65a8358d6",
  "type": "Type value",
  "displayName": "Display Name value"
}
```

