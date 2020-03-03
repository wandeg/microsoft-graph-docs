---
title: "Create chatActivityStatistics"
description: "Create a new chatActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create chatActivityStatistics

Namespace: microsoft.graph

Create a new [chatActivityStatistics](../resources/chatactivitystatistics.md) object.

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
POST ** Collection URI for microsoft.graph.chatActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [chatActivityStatistics](../resources/chatactivitystatistics.md) object.

The following table shows the properties that are required when you create the [chatActivityStatistics](../resources/chatactivitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activitystatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|afterHours|Duration||



## Response
If successful, this method returns a `201 Created` response code and a [chatActivityStatistics](../resources/chatactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_chatactivitystatistics_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.chatActivityStatistics not found
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.chatActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M55.0810357S",
  "afterHours": "-PT1M34.3242013S"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatactivitystatistics"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.chatActivityStatistics",
  "id": "bc35ab08-ab08-bc35-08ab-35bc08ab35bc",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "-PT1M55.0810357S",
  "afterHours": "-PT1M34.3242013S"
}
```

