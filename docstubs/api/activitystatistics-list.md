---
title: "List activityStatistics"
description: "Get a list of the activityStatistics objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List activityStatistics

Namespace: microsoft.graph

Get a list of the [activityStatistics](../resources/activitystatistics.md) objects and their properties.

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
GET /activitystatistics
GET /invitations/{invitationsId}/invitedUser/analytics/activityStatistics
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
If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}
-->
``` http
GET https://graph.microsoft.com/beta/activitystatistics
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.activitystatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityStatistics",
      "id": "5500b1a5-b1a5-5500-a5b1-0055a5b10055",
      "activity": "String",
      "startDate": "Date",
      "endDate": "Date",
      "timeZoneUsed": "Time Zone Used value",
      "duration": "PT1M49.5464392S"
    }
  ]
}
```

