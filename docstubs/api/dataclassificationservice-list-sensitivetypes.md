---
title: "List sensitiveTypes"
description: "Get the sensitiveTypes from the sensitiveTypes navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sensitiveTypes

Namespace: microsoft.graph

Get the sensitiveTypes from the sensitiveTypes navigation property.

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
GET /dataClassification/sensitiveTypes
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
If successful, this method returns a `200 OK` response code and a collection of [sensitiveType](../resources/sensitivetype.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sensitivetype"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitiveTypes
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sensitivetype)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sensitiveType",
      "id": "75f5c30b-c30b-75f5-0bc3-f5750bc3f575",
      "name": "Name value",
      "description": "Description value",
      "rulePackageId": "Rule Package Id value",
      "rulePackageType": "Rule Package Type value",
      "publisherName": "Publisher Name value",
      "state": "State value",
      "scope": "String"
    }
  ]
}
```

