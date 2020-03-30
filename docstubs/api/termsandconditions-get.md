---
title: "Get termsAndConditions"
description: "Read properties and relationships of the termsAndConditions object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get termsAndConditions

Namespace: microsoft.graph

Read properties and relationships of the [termsAndConditions](../resources/termsandconditions.md) object.

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
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
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
If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/termsandconditions.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_termsandconditions"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "b667659b-659b-b667-9b65-67b69b6567b6",
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
    "modifiedDateTime": "2016-12-31T23:59:25.7728733+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```

