---
title: "Get featureRolloutPolicy"
description: "Read properties and relationships of the featureRolloutPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get featureRolloutPolicy

Namespace: microsoft.graph

Read properties and relationships of the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.

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
GET /directory/featureRolloutPolicies/{featureRolloutPolicyId}
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
If successful, this method returns a `200 OK` response code and [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/{featureRolloutPolicyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 305

{
  "value": {
    "@odata.type": "#microsoft.graph.featureRolloutPolicy",
    "id": "a4cd56f0-56f0-a4cd-f056-cda4f056cda4",
    "displayName": "Display Name value",
    "description": "Description value",
    "feature": "String",
    "isEnabled": true,
    "isAppliedToOrganization": true
  }
}
```

