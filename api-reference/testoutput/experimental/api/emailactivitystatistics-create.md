---
title: "Create emailActivityStatistics"
description: "Create a new emailActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create emailActivityStatistics

Create a new [emailActivityStatistics](../resources/emailactivitystatistics.md) object.

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
POST ** Collection URI for microsoft.graph.emailActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the emailActivityStatistics object.

The following table shows the properties that are required when you create the emailActivityStatistics.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activityStatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|afterHours|Duration||
|readEmail|Duration||
|sentEmail|Duration||



## Response
If successful, this method returns a `201 Created` response code and a [emailActivityStatistics](../resources/emailactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_emailactivitystatistics_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.emailActivityStatistics not found
Content-type: application/json
Content-length: 318

{
  "@odata.type": "#microsoft.graph.emailActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S",
  "afterHours": "PT21.1795365S",
  "readEmail": "-PT3M11.7567899S",
  "sentEmail": "PT1M11.5133279S"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailactivitystatistics"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 367

{
  "@odata.type": "#microsoft.graph.emailActivityStatistics",
  "id": "9b030e25-0e25-9b03-250e-039b250e039b",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S",
  "afterHours": "PT21.1795365S",
  "readEmail": "-PT3M11.7567899S",
  "sentEmail": "PT1M11.5133279S"
}
```

