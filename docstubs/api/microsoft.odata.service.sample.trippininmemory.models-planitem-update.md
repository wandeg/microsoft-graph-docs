---
title: "Update planItem"
description: "Update the properties of a planItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update planItem

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.

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

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.

The following table shows the properties that are required when you create the [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md).

|Property|Type|Description|
|:---|:---|:---|
|planItemId|Int32||
|confirmationCode|String||
|startsAtDateTime|DateTimeOffset||
|endsAtDateTime|DateTimeOffset||
|duration|Duration||



## Response
If successful, this method returns a `200 OK` response code and an updated [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_planitem"
}
-->
``` http

```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem",
  "planItemId": 10,
  "confirmationCode": "Confirmation Code value",
  "startsAtDateTime": "2017-01-01T00:02:51.9468808+03:00",
  "endsAtDateTime": "2017-01-01T00:02:30.5158823+03:00",
  "duration": "-PT4.4893728S"
}
```

