---
title: "Add appRoleAssignments"
description: "Add appRoleAssignments by posting to the appRoleAssignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appRoleAssignments

Namespace: microsoft.graph

Add appRoleAssignments by posting to the appRoleAssignments collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /groups/{groupsId}/appRoleAssignments/$ref
POST /me/joinedGroups/{groupId}/appRoleAssignments/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [appRoleAssignment](../resources/approleassignment.md) object.

The following table shows the properties that are required when you create the [appRoleAssignment](../resources/approleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appRoleId|Guid||
|creationTimestamp|DateTimeOffset||
|principalDisplayName|String||
|principalId|Guid||
|principalType|String||
|resourceDisplayName|String||
|resourceId|Guid||



## Response
If successful, this method returns a `201 Created` response code and a [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_approleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/appRoleAssignments
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "cf4673b9-73b9-cf46-b973-46cfb97346cf",
  "creationTimestamp": "2016-12-31T23:59:16.223907+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "d5b695e0-95e0-d5b6-e095-b6d5e095b6d5",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "7989ade7-ade7-7989-e7ad-8979e7ad8979"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 499

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "97175786-5786-9717-8657-179786571797",
  "appRoleId": "cf4673b9-73b9-cf46-b973-46cfb97346cf",
  "creationTimestamp": "2016-12-31T23:59:16.223907+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "d5b695e0-95e0-d5b6-e095-b6d5e095b6d5",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "7989ade7-ade7-7989-e7ad-8979e7ad8979"
}
```

