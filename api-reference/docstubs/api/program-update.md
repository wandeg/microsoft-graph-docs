---
title: "Update program"
description: "Update the properties of a program object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update program

Namespace: microsoft.graph

Update the properties of a [program](../resources/program.md) object.

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
PATCH /programs/{programsId}
PATCH /programControls/{programControlsId}/program
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [program](../resources/program.md) object.

The following table shows the properties that are required when you create the [program](../resources/program.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|



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
Content-Type: application/json
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
{
  "@odata.type": "#microsoft.graph.program",
  "id": "0cde1fe6-1fe6-0cde-e61f-de0ce61fde0c",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

