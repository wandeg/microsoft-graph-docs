---
title: "getPolicySets"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getPolicySets

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
POST /deviceAppManagement/policySets/getPolicySets
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|policySetIds|String collection||



## Response
If successful, this action returns a `200 OK` response code and a [policySet](../resources/policyset.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "policyset_getpolicysets"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/policySets/getPolicySets

Content-type: application/json
Content-length: 58

{
  "policySetIds": [
    "Policy Set Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "b9715cea-5cea-b971-ea5c-71b9ea5c71b9",
      "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
      "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
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

