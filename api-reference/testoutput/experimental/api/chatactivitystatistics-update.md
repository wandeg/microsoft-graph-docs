---
title: "Update chatActivityStatistics"
description: "Update the properties of a chatActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update chatActivityStatistics

Update the properties of a [chatActivityStatistics](../resources/chatactivitystatistics.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.chatActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [chatActivityStatistics](../resources/chatActivityStatistics.md) object.

The following table shows the properties that are required when you create the [chatActivityStatistics](../resources/chatactivitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activityStatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|afterHours|Duration||



## Response
If successful, this method returns a `200 OK` response code and an updated [chatActivityStatistics](../resources/chatactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_chatactivitystatistics"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.chatActivityStatistics not found
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.chatActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S",
  "afterHours": "PT21.1795365S"
}
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
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.chatActivityStatistics",
  "id": "317b47fc-47fc-317b-fc47-7b31fc477b31",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S",
  "afterHours": "PT21.1795365S"
}
```

