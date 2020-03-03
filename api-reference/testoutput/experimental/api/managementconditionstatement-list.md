---
title: "List managementConditionStatements"
description: "List properties and relationships of the managementConditionStatement objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managementConditionStatements

Namespace: microsoft.graph

List properties and relationships of the [managementConditionStatement](../resources/managementconditionstatement.md) objects.

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
GET /deviceManagement/managementConditionStatements
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managementConditionStatement](../resources/managementconditionstatement.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managementconditionstatement"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/managementConditionStatements
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managementconditionstatement)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "443eae60-ae60-443e-60ae-3e4460ae3e44",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "String"
      ]
    }
  ]
}
```

