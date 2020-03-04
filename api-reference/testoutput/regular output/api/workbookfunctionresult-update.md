---
title: "Update workbookFunctionResult"
description: "Update the properties of a workbookFunctionResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookFunctionResult

Namespace: microsoft.graph

Update the properties of a [workbookFunctionResult](../resources/workbookfunctionresult.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookFunctionResult not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookFunctionResult](../resources/workbookfunctionresult.md) object.

The following table shows the properties that are required when you create the [workbookFunctionResult](../resources/workbookfunctionresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|error|String||
|value|[Json](../resources/json.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookFunctionResult](../resources/workbookfunctionresult.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookfunctionresult"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookFunctionResult not found
Content-type: application/json
Content-length: 154

{
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "error": "Error value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
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
Content-Length: 203

{
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "id": "b41bdfb7-dfb7-b41b-b7df-1bb4b7df1bb4",
  "error": "Error value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

