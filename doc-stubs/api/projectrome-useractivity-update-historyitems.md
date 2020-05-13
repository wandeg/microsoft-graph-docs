---
title: "Update historyItems"
description: "Update the properties of a historyItems object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update historyItems

Namespace: microsoft.graph

Update the properties of a historyItems object.

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
PATCH /users/{usersId}/activities/{userActivityId}/historyItems
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [activityHistoryItem](../resources/projectrome-activityhistoryitem.md) object.

The following table shows the properties that are required when you create the [activityHistoryItem](../resources/projectrome-activityhistoryitem.md).

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

If successful, this method returns a `200 OK` response code and an updated [activityHistoryItem](../resources/projectrome-activityhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_historyitems"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/activities/{userActivityId}/historyItems
Content-Type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "status": "String",
  "activeDurationSeconds": "Integer",
  "lastActiveDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "startedDateTime": "String (timestamp)",
  "userTimezone": "String"
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
  "id": "368c8aac-8aac-368c-ac8a-8c36ac8a8c36",
  "status": "String",
  "activeDurationSeconds": "Integer",
  "createdDateTime": "String (timestamp)",
  "lastActiveDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "startedDateTime": "String (timestamp)",
  "userTimezone": "String"
}
```

