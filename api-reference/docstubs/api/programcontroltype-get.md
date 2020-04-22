---
title: "Get programControlType"
description: "Read properties and relationships of a programControlType object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get programControlType

Namespace: microsoft.graph

Read properties and relationships of a [programControlType](../resources/programcontroltype.md) object.

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
GET /programControlTypes/{programControlTypesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [programControlType](../resources/programcontroltype.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/programControlTypes/{programControlTypesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.programControlType",
    "id": "7089a698-a698-7089-98a6-897098a68970",
    "controlTypeGroupId": "Control Type Group Id value",
    "displayName": "Display Name value"
  }
}
```

