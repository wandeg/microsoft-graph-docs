---
title: "Create resourceSpecificPermissionGrant"
description: "Create a new resourceSpecificPermissionGrant object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create resourceSpecificPermissionGrant

Namespace: Microsoft.DirectoryServices

Create a new [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) object.

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
POST /permissionGrants
POST /groups/{groupsId}/permissionGrants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) object.

The following table shows the properties that are required when you create the [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|clientId|String|**TODO: Add Description**|
|clientAppId|String|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|
|permissionType|String|**TODO: Add Description**|
|permission|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_resourcespecificpermissiongrant_from_permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/changelog/permissionGrants
Content-Type: application/json
Content-length: 347

{
  "@odata.type": "#Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
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
  "@odata.type": "microsoft.directoryservices.resourcespecificpermissiongrant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
  "id": "d4714e75-4e75-d471-754e-71d4754e71d4",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
}
```

