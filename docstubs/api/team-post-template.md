---
title: "Add template"
description: "Add template by posting to the template collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add template

Namespace: microsoft.graph

Add template by posting to the template collection.

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
POST /teams/{teamsId}/template/$ref
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/template/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [teamsTemplate](../resources/teamstemplate.md) object.

The following table shows the properties that are required when you create the [teamsTemplate](../resources/teamstemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `204 No Content` response code and a [teamsTemplate](../resources/teamstemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_teamstemplate_from_teamstemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamsId}/template/$ref
Content-Type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.teamsTemplate"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamstemplate"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.teamsTemplate",
  "id": "4fe762e1-62e1-4fe7-e162-e74fe162e74f"
}
```

