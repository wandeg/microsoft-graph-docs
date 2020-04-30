---
title: "Update activities"
description: "Update the properties of an activities object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update activities

Namespace: microsoft.graph

Update the properties of an activities object.

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
PATCH /me/activities
PATCH /users/{usersId}/activities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userActivity](../resources/useractivity.md) object.

The following table shows the properties that are required when you create the [userActivity](../resources/useractivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|visualElements|[visualInfo](../resources/visualinfo.md)|**TODO: Add Description**|
|activitySourceHost|String|**TODO: Add Description**|
|activationUrl|String|**TODO: Add Description**|
|appActivityId|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|fallbackUrl|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|userTimezone|String|**TODO: Add Description**|
|contentInfo|[Json](../resources/json.md)|**TODO: Add Description**|
|status|status|**TODO: Add Description**. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [userActivity](../resources/useractivity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_activities"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/activities
Content-Type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.userActivity",
  "visualElements": {
    "@odata.type": "microsoft.graph.visualInfo"
  },
  "activitySourceHost": "String",
  "activationUrl": "String",
  "appActivityId": "String",
  "appDisplayName": "String",
  "contentUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "fallbackUrl": "String",
  "userTimezone": "String",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
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
  "@odata.type": "#microsoft.graph.userActivity",
  "id": "e71b5577-5577-e71b-7755-1be777551be7",
  "visualElements": {
    "@odata.type": "microsoft.graph.visualInfo"
  },
  "activitySourceHost": "String",
  "activationUrl": "String",
  "appActivityId": "String",
  "appDisplayName": "String",
  "contentUrl": "String",
  "createdDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "fallbackUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "userTimezone": "String",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

