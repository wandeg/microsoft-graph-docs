---
title: "List featureRolloutPolicies"
description: "Get the featureRolloutPolicies from the featureRolloutPolicies navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List featureRolloutPolicies

Namespace: microsoft.graph

Get the featureRolloutPolicies from the featureRolloutPolicies navigation property.

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
GET /directory/featureRolloutPolicies
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
If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.featurerolloutpolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.featureRolloutPolicy",
      "id": "726c93bb-93bb-726c-bb93-6c72bb936c72",
      "displayName": "Display Name value",
      "description": "Description value",
      "feature": "String",
      "isEnabled": true,
      "isAppliedToOrganization": true
    }
  ]
}
```

