---
title: "Get informationProtectionPolicy"
description: "Read properties and relationships of the informationProtectionPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get informationProtectionPolicy

Namespace: microsoft.graph

Read properties and relationships of the [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.

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
GET /informationProtection/policy
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
If successful, this method returns a `200 OK` response code and [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/policy
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 141

{
  "value": {
    "@odata.type": "#microsoft.graph.informationProtectionPolicy",
    "id": "a7c2f5e7-f5e7-a7c2-e7f5-c2a7e7f5c2a7"
  }
}
```

