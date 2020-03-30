---
title: "Create program"
description: "Create a new program object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create program

Namespace: microsoft.graph

Create a new [program](../resources/program.md) object.

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
POST /programs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [program](../resources/program.md) object.

The following table shows the properties that are required when you create the [program](../resources/program.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||



## Response
If successful, this method returns a `201 Created` response code and a [program](../resources/program.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}
-->
``` http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.program",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.program",
  "id": "f1b66fea-6fea-f1b6-ea6f-b6f1ea6fb6f1",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

