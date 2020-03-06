---
title: "Add activityStatistics"
description: "Add activityStatistics by posting to the activityStatistics collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add activityStatistics

Namespace: microsoft.graph

Add activityStatistics by posting to the activityStatistics collection.

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
POST /me/analytics/activityStatistics/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [activityStatistics](../resources/activitystatistics.md) object.

The following table shows the properties that are required when you create the [activityStatistics](../resources/activitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration|. Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date||
|endDate|Date||
|timeZoneUsed|String||
|duration|Duration||



## Response
If successful, this method returns a `201 Created` response code and a [activityStatistics](../resources/activitystatistics.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_activitystatistics_from_activitystatistics"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/analytics/activityStatistics
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.activityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M8.1281301S"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activitystatistics"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.activityStatistics",
  "id": "ae94736b-736b-ae94-6b73-94ae6b7394ae",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M8.1281301S"
}
```

