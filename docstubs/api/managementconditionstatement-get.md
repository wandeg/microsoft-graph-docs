---
title: "Get managementConditionStatement"
description: "Read properties and relationships of the managementConditionStatement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get managementConditionStatement

Namespace: microsoft.graph

Read properties and relationships of the [managementConditionStatement](../resources/managementconditionstatement.md) object.

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
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}
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
If successful, this method returns a `200 OK` response code and [managementConditionStatement](../resources/managementconditionstatement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_managementconditionstatement"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "value": {
    "@odata.type": "#microsoft.graph.managementConditionStatement",
    "id": "3d5029fc-29fc-3d50-fc29-503dfc29503d",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "modifiedDateTime": "2017-01-01T00:01:10.7827862+00:00",
    "expression": {
      "@odata.type": "microsoft.graph.managementConditionExpression"
    },
    "eTag": "ETag value",
    "applicablePlatforms": [
      "String"
    ]
  }
}
```

