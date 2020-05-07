---
title: "Get timeOff"
description: "Read the properties and relationships of a timeOff object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get timeOff

Namespace: microsoft.graph

Read the properties and relationships of a [timeOff](../resources/timeoff.md) object.

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
GET /teams/{teamsId}/schedule/timesOff/{timeOffId}
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

If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_timeoff"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule/timesOff/{timeOffId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.timeOff",
    "id": "f1040c0c-0c0c-f104-0c0c-04f10c0c04f1",
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "sharedTimeOff": {
      "@odata.type": "microsoft.graph.timeOffItem"
    },
    "draftTimeOff": {
      "@odata.type": "microsoft.graph.timeOffItem"
    },
    "userId": "String"
  }
}
```

