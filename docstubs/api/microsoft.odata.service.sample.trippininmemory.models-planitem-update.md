---
title: "Update PlanItem"
description: "Update the properties of a PlanItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update PlanItem

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.

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
In the request body, supply a JSON representation for the [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.

The following table shows the properties that are required when you create the [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md).

|Property|Type|Description|
|:---|:---|:---|
|PlanItemId|Int32||
|ConfirmationCode|String||
|StartsAt|DateTimeOffset||
|EndsAt|DateTimeOffset||
|Duration|Duration||



## Response
If successful, this method returns a `200 OK` response code and an updated [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_planitem"
}
-->
``` http

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
Content-Length: 296

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.PlanItem",
  "PlanItemId": 10,
  "ConfirmationCode": "Confirmation Code value",
  "StartsAt": "2017-01-01T00:01:10.6216491+03:00",
  "EndsAt": "2017-01-01T00:02:07.8652631+03:00",
  "Duration": "-PT3M12.1584941S"
}
```

