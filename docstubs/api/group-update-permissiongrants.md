---
title: "Update permissionGrants"
description: "Update the properties of a permissionGrants object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update permissionGrants

Namespace: microsoft.graph

Update the properties of a permissionGrants object.

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
PATCH /groups/{groupsId}/permissionGrants
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/permissionGrants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

The following table shows the properties that are required when you create the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|clientId|String|**TODO: Add Description**|
|clientAppId|String|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|
|permissionType|String|**TODO: Add Description**|
|permission|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_permissiongrants"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/permissionGrants
Content-Type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "deletedDateTime": "2016-12-31T23:56:33.098707+03:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "95cdc9a4-c9a4-95cd-a4c9-cd95a4c9cd95",
  "deletedDateTime": "2016-12-31T23:56:33.098707+03:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
}
```

