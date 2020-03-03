---
title: "Get programControlType"
description: "Read properties and relationships of the programControlType object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get programControlType

Namespace: microsoft.graph

Read properties and relationships of the [programControlType](../resources/programcontroltype.md) object.

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
GET /programControlTypes/{programControlTypesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [programControlType](../resources/programcontroltype.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}
-->
``` http
GET https://graph.microsoft.com/localtest/programControlTypes/{programControlTypesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "value": {
    "@odata.type": "#microsoft.graph.programControlType",
    "id": "7a38ef3d-ef3d-7a38-3def-387a3def387a",
    "controlTypeGroupId": "Control Type Group Id value",
    "displayName": "Display Name value"
  }
}
```

