---
title: "Get yammerGroupsActivityDetail"
description: "Read the properties and relationships of a yammerGroupsActivityDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get yammerGroupsActivityDetail

Namespace: microsoft.graph

Read the properties and relationships of a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

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
GET /yammerGroupsActivityDetail
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

If successful, this method returns a `200 OK` response code and a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_yammergroupsactivitydetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/yammerGroupsActivityDetail
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
    "id": "bf16bbaa-bbaa-bf16-aabb-16bfaabb16bf",
    "reportRefreshDate": "Date",
    "groupDisplayName": "String",
    "isDeleted": "Boolean",
    "ownerPrincipalName": "String",
    "lastActivityDate": "Date",
    "groupType": "String",
    "office365Connected": "Boolean",
    "memberCount": "Integer",
    "postedCount": "Integer",
    "readCount": "Integer",
    "likedCount": "Integer",
    "networkDisplayName": "String",
    "reportPeriod": "String"
  }
}
```

