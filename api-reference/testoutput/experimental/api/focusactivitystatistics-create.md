---
title: "Create focusActivityStatistics"
description: "Create a new focusActivityStatistics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create focusActivityStatistics

Create a new [focusActivityStatistics](../resources/focusactivitystatistics.md) object.

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
POST ** Collection URI for microsoft.graph.focusActivityStatistics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the focusActivityStatistics object.

The following table shows the properties that are required when you create the focusActivityStatistics.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activityStatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|duration|Duration| Inherited from [activityStatistics](../resources/activityStatistics.md)|



## Response
If successful, this method returns a `201 Created` response code and a [focusActivityStatistics](../resources/focusactivitystatistics.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_focusactivitystatistics_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.focusActivityStatistics not found
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.focusActivityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.focusactivitystatistics"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.focusActivityStatistics",
  "id": "f835d8b2-d8b2-f835-b2d8-35f8b2d835f8",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "Time Zone Used value",
  "duration": "PT3M27.7161587S"
}
```

