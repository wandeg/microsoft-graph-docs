---
title: "Get trustFramework"
description: "Read properties and relationships of a trustFramework object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get trustFramework

Namespace: microsoft.cpim.api.dataModels

Read properties and relationships of a [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /trustFramework
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_trustframework"
}
-->
``` http
GET https://graph.microsoft.com/beta/trustFramework
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.dataModels.trustFramework"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.cpim.api.dataModels.trustFramework",
    "id": "1579292e-292e-1579-2e29-79152e297915"
  }
}
```

