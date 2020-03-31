---
title: "Get policySet"
description: "Read properties and relationships of the policySet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get policySet

Namespace: microsoft.graph

Read properties and relationships of the [policySet](../resources/policyset.md) object.

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
GET /deviceAppManagement/policySets/{policySetId}
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
If successful, this method returns a `200 OK` response code and [policySet](../resources/policyset.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_policyset"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.policySet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 525

{
  "value": {
    "@odata.type": "#microsoft.graph.policySet",
    "id": "d56ec225-c225-d56e-25c2-6ed525c26ed5",
    "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "status": "String",
    "errorCode": "String",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ],
    "roleScopeTags": [
      "Role Scope Tags value"
    ]
  }
}
```

