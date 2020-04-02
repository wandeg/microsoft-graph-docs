---
title: "Create PlanItems"
description: "Create PlanItems by posting to the PlanItems collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create PlanItems

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create PlanItems by posting to the PlanItems collection.

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
POST /Me/Trips/{TripId}/PlanItems/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_planitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Me/Trips/{TripId}/PlanItems
Content-type: application/json
Content-length: 294

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.PlanItem",
  "PlanItemId": 10,
  "ConfirmationCode": "Confirmation Code value",
  "StartsAt": "2016-12-31T23:59:33.2560191+03:00",
  "EndsAt": "2017-01-01T00:00:38.034091+03:00",
  "Duration": "-PT1M2.3081203S"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.odata.service.sample.trippininmemory.models.planitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.PlanItem",
  "PlanItemId": 10,
  "ConfirmationCode": "Confirmation Code value",
  "StartsAt": "2016-12-31T23:59:33.2560191+03:00",
  "EndsAt": "2017-01-01T00:00:38.034091+03:00",
  "Duration": "-PT1M2.3081203S"
}
```

