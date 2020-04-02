---
title: "List PlanItems"
description: "Get the PlanItems from the PlanItems navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List PlanItems

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Get the PlanItems from the PlanItems navigation property.

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
GET /Me/Trips/{TripId}/PlanItems
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
If successful, this method returns a `200 OK` response code and a collection of [PlanItem](../resources/planitem.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_planitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/Me/Trips/{TripId}/PlanItems
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.odata.service.sample.trippininmemory.models.planitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 351

{
  "value": [
    {
      "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.PlanItem",
      "PlanItemId": 10,
      "ConfirmationCode": "Confirmation Code value",
      "StartsAt": "2016-12-31T23:59:33.2560191+03:00",
      "EndsAt": "2017-01-01T00:00:38.034091+03:00",
      "Duration": "-PT1M2.3081203S"
    }
  ]
}
```

