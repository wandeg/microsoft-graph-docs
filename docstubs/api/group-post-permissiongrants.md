---
title: "Add permissionGrants"
description: "Add permissionGrants by posting to the permissionGrants collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add permissionGrants

Namespace: microsoft.graph

Add permissionGrants by posting to the permissionGrants collection.

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
POST /groups/{groupsId}/permissionGrants/$ref
POST /me/joinedGroups/{groupId}/permissionGrants/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_resourcespecificpermissiongrant_from_permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/permissionGrants
Content-Type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "deletedDateTime": "2016-12-31T23:58:28.3197258+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.resourcespecificpermissiongrant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "819e7522-7522-819e-2275-9e8122759e81",
  "deletedDateTime": "2016-12-31T23:58:28.3197258+03:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
}
```

