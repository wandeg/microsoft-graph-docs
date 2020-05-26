---
title: "Create yammerGroupsActivityDetail"
description: "Create a new yammerGroupsActivityDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create yammerGroupsActivityDetail

Namespace: microsoft.graph

Create a new [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

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
POST ** Collection URI for microsoft.graph.yammerGroupsActivityDetail not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

The following table shows the properties that are required when you create the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date|**TODO: Add Description**|
|groupDisplayName|String|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description**|
|ownerPrincipalName|String|**TODO: Add Description**|
|lastActivityDate|Date|**TODO: Add Description**|
|groupType|String|**TODO: Add Description**|
|office365Connected|Boolean|**TODO: Add Description**|
|memberCount|Int64|**TODO: Add Description**|
|postedCount|Int64|**TODO: Add Description**|
|readCount|Int64|**TODO: Add Description**|
|likedCount|Int64|**TODO: Add Description**|
|networkDisplayName|String|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_yammergroupsactivitydetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.yammerGroupsActivityDetail not found
Content-Type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
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
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammergroupsactivitydetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

