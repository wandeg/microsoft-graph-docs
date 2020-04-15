---
title: "Get planItem"
description: "Read properties and relationships of the planItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get planItem

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Read properties and relationships of the [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.

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
If successful, this method returns a `200 OK` response code and [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_planitem"
}
-->
``` http

```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": {
    "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem",
    "planItemId": 10,
    "confirmationCode": "Confirmation Code value",
    "startsAtDateTime": "2017-01-01T00:02:51.9468808+03:00",
    "endsAtDateTime": "2017-01-01T00:02:30.5158823+03:00",
    "duration": "-PT4.4893728S"
  }
}
```

