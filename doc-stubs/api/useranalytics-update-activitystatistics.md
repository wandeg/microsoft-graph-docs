---
title: "Update activityStatistics"
description: "Update the properties of an activityStatistics object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update activityStatistics

Namespace: microsoft.graph

Update the properties of an activityStatistics object.

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
PATCH ** Collection URI for microsoft.graph.activityStatistics not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [activityStatistics](../resources/activitystatistics.md) object.

The following table shows the properties that are required when you create the [activityStatistics](../resources/activitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activity|analyticsActivityType|**TODO: Add Description**. Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|startDate|Date|**TODO: Add Description**|
|endDate|Date|**TODO: Add Description**|
|timeZoneUsed|String|**TODO: Add Description**|
|duration|Duration|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [activityStatistics](../resources/activitystatistics.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_activitystatistics"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.activityStatistics not found
Content-Type: application/json
Content-length: 196

{
  "@odata.type": "#microsoft.graph.activityStatistics",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.activityStatistics",
  "id": "29ac3b30-3b30-29ac-303b-ac29303bac29",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)"
}
```

