---
title: "getManagementConditionStatementsForPlatform"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getManagementConditionStatementsForPlatform

Namespace: microsoft.graph



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
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|platform|Enumeration||



## Response
If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/managementconditionstatement.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "managementconditionstatement_getmanagementconditionstatementsforplatform"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
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
Content-Length: 568

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "63bc5778-5778-63bc-7857-bc637857bc63",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "modifiedDateTime": "2016-12-31T23:57:56.5934914+03:00",
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

