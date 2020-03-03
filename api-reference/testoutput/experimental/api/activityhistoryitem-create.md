---
title: "Create activityHistoryItem"
description: "Create a new activityHistoryItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create activityHistoryItem

Namespace: microsoft.graph

Create a new [activityHistoryItem](../resources/activityhistoryitem.md) object.

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
POST /me/activities/{userActivityId}/historyItems
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [activityHistoryItem](../resources/activityhistoryitem.md) object.

The following table shows the properties that are required when you create the [activityHistoryItem](../resources/activityhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|activeDurationSeconds|Int32||
|createdDateTime|DateTimeOffset||
|lastActiveDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|startedDateTime|DateTimeOffset||
|userTimezone|String||



## Response
If successful, this method returns a `201 Created` response code and a [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_activityhistoryitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/activities/{userActivityId}/historyItems
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "status": "String",
  "activeDurationSeconds": 5,
  "lastActiveDateTime": "2016-12-31T23:58:54.0663658+03:00",
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "startedDateTime": "2016-12-31T23:57:57.4958527+03:00",
  "userTimezone": "User Timezone value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityhistoryitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 511

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "id": "8f247e5d-7e5d-8f24-5d7e-248f5d7e248f",
  "status": "String",
  "activeDurationSeconds": 5,
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastActiveDateTime": "2016-12-31T23:58:54.0663658+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "startedDateTime": "2016-12-31T23:57:57.4958527+03:00",
  "userTimezone": "User Timezone value"
}
```

