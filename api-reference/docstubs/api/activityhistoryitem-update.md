---
title: "Update activityHistoryItem"
description: "Update the properties of an activityHistoryItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update activityHistoryItem

Namespace: microsoft.graph

Update the properties of an [activityHistoryItem](../resources/activityhistoryitem.md) object.

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
PATCH /invitations/{invitationsId}/invitedUser/activities/{userActivityId}/historyItems/{activityHistoryItemId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [activityHistoryItem](../resources/activityhistoryitem.md) object.

The following table shows the properties that are required when you create the [activityHistoryItem](../resources/activityhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|status|**TODO: Add Description**. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|activeDurationSeconds|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastActiveDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|startedDateTime|DateTimeOffset|**TODO: Add Description**|
|userTimezone|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_activityhistoryitem"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/activities/{userActivityId}/historyItems/{activityHistoryItemId}
Content-Type: application/json
Content-length: 338

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "status": "String",
  "activeDurationSeconds": 5,
  "lastActiveDateTime": "2017-01-01T00:02:01.5517519+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "startedDateTime": "2017-01-01T00:03:12.189456+03:00",
  "userTimezone": "User Timezone value"
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
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "id": "2cffeada-eada-2cff-daea-ff2cdaeaff2c",
  "status": "String",
  "activeDurationSeconds": 5,
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastActiveDateTime": "2017-01-01T00:02:01.5517519+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "startedDateTime": "2017-01-01T00:03:12.189456+03:00",
  "userTimezone": "User Timezone value"
}
```

