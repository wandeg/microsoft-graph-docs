---
title: "Create planItems"
description: "Create planItems by posting to the planItems collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create planItems

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create planItems by posting to the planItems collection.

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
POST /me/trips/{tripId}/planItems/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.

The following table shows the properties that are required when you create the [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md).

|Property|Type|Description|
|:---|:---|:---|
|planItemId|Int32||
|confirmationCode|String||
|startsAt|DateTimeOffset||
|endsAt|DateTimeOffset||
|duration|Duration||



## Response
If successful, this method returns a `201 Created` response code and a [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_planitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/trips/{tripId}/planItems
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem",
  "planItemId": 10,
  "confirmationCode": "Confirmation Code value",
  "startsAt": "2016-12-31T23:56:46.9049138+03:00",
  "endsAt": "2016-12-31T23:57:07.6482324+03:00",
  "duration": "PT3M16.6801712S"
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
Content-Length: 295

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem",
  "planItemId": 10,
  "confirmationCode": "Confirmation Code value",
  "startsAt": "2016-12-31T23:56:46.9049138+03:00",
  "endsAt": "2016-12-31T23:57:07.6482324+03:00",
  "duration": "PT3M16.6801712S"
}
```

