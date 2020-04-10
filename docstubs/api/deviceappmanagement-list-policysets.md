---
title: "List policySets"
description: "Get the policySets from the policySets navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List policySets

Namespace: microsoft.graph

Get the policySets from the policySets navigation property.

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
GET /deviceAppManagement/policySets
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
If successful, this method returns a `200 OK` response code and a collection of [policySet](../resources/policyset.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_policyset"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.policyset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySet",
      "id": "0af8323b-323b-0af8-3b32-f80a3b32f80a",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
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
  ]
}
```

