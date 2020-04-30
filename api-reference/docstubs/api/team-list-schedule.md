---
title: "List schedule"
description: "Get the schedules from the schedule navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List schedule

Namespace: microsoft.graph

Get the schedules from the schedule navigation property.

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
GET /teams/{teamsId}/schedule
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [schedule](../resources/schedule.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_schedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.schedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.schedule",
      "id": "ceb7e724-e724-ceb7-24e7-b7ce24e7b7ce",
      "enabled": "Boolean",
      "timeZone": "String",
      "provisionStatus": "String",
      "provisionStatusCode": "String",
      "workforceIntegrationIds": [
        "String"
      ],
      "timeClockEnabled": "Boolean",
      "openShiftsEnabled": "Boolean",
      "swapShiftsRequestsEnabled": "Boolean",
      "offerShiftRequestsEnabled": "Boolean",
      "timeOffRequestsEnabled": "Boolean"
    }
  ]
}
```

