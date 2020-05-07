---
title: "List activity"
description: "Get the userActivities from the activity navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List activity

Namespace: microsoft.graph

Get the userActivities from the activity navigation property.

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
GET /users/{usersId}/activities/{userActivityId}/historyItems/{activityHistoryItemId}/activity
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [userActivity](../resources/useractivity.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_useractivity"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/activities/{userActivityId}/historyItems/{activityHistoryItemId}/activity
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.useractivity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userActivity",
      "id": "47a30165-0165-47a3-6501-a3476501a347",
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
  ]
}
```

