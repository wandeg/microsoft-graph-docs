---
title: "Create taskGroups"
description: "Create a new taskGroups object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create taskGroups

Namespace: microsoft.graph

Create a new taskGroups object.

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
POST /invitations/{invitationsId}/invitedUser/outlook/taskGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

The following table shows the properties that are required when you create the [outlookTaskGroup](../resources/outlooktaskgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|changeKey|String|**TODO: Add Description**|
|isDefaultGroup|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|groupKey|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/outlook/taskGroups
Content-Type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "be947289-7289-be94-8972-94be897294be"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlooktaskgroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "id": "230c3936-3936-230c-3639-0c2336390c23",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "be947289-7289-be94-8972-94be897294be"
}
```

