---
title: "Update program"
description: "Update the properties of a program object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update program

Namespace: microsoft.graph

Update the properties of a [program](../resources/program.md) object.

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
PATCH /programs/{programsId}
PATCH /programControls/{programControlsId}/program
PATCH /programs/{programsId}/controls/{programControlId}/program
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [program](../resources/program.md) object.

The following table shows the properties that are required when you create the [program](../resources/program.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [program](../resources/program.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_program"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/programs/{programsId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.program",
  "displayName": "Display Name value",
  "description": "Description value"
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
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.program",
  "id": "dba9ab0c-ab0c-dba9-0cab-a9db0caba9db",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

