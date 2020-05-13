---
title: "List timeOffRequests"
description: "Get the timeOffRequests from the timeOffRequests navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List timeOffRequests

Namespace: microsoft.graph

Get the timeOffRequests from the timeOffRequests navigation property.

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
GET /teams/{teamsId}/schedule/timeOffRequests
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

If successful, this method returns a `200 OK` response code and a collection of [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/{teamsId}/schedule/timeOffRequests
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.timeoffrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.timeOffRequest",
      "id": "8b472da5-2da5-8b47-a52d-478ba52d478b",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "assignedTo": "String",
      "state": "String",
      "senderMessage": "String",
      "senderDateTime": "String (timestamp)",
      "managerActionMessage": "String",
      "managerActionDateTime": "String (timestamp)",
      "senderUserId": "String",
      "managerUserId": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "timeOffReasonId": "String"
    }
  ]
}
```

