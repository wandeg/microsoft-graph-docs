---
title: "Update tokenLifetimePolicy"
description: "Update the properties of a tokenLifetimePolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update tokenLifetimePolicy

Namespace: microsoft.graph

Update the properties of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.

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
PATCH /policies/tokenLifetimePolicies/{tokenLifetimePolicyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.

The following table shows the properties that are required when you create the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|definition|String collection| Inherited from [stsPolicy](../resources/stspolicy.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stspolicy.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_tokenlifetimepolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{tokenLifetimePolicyId}
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.tokenLifetimePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.tokenLifetimePolicy",
  "id": "a0d27219-7219-a0d2-1972-d2a01972d2a0",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```

