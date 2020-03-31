---
title: "Get sensitiveType"
description: "Read properties and relationships of the sensitiveType object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sensitiveType

Namespace: microsoft.graph

Read properties and relationships of the [sensitiveType](../resources/sensitivetype.md) object.

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
GET /dataClassification/sensitiveTypes/{sensitiveTypeId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [sensitiveType](../resources/sensitivetype.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sensitivetype"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitiveTypes/{sensitiveTypeId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitiveType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.sensitiveType",
    "id": "1f9caf48-af48-1f9c-48af-9c1f48af9c1f",
    "name": "Name value",
    "description": "Description value",
    "rulePackageId": "Rule Package Id value",
    "rulePackageType": "Rule Package Type value",
    "publisherName": "Publisher Name value",
    "state": "State value",
    "scope": "String"
  }
}
```

