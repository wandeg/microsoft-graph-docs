---
title: "Update appRoleAssignedTo"
description: "Update the properties of an appRoleAssignedTo object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update appRoleAssignedTo

Namespace: Microsoft.DirectoryServices

Update the properties of an appRoleAssignedTo object.

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
PATCH /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) object.

The following table shows the properties that are required when you create the [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|appRoleId|Guid|**TODO: Add Description**|
|creationTimestamp|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|principalDisplayName|String|**TODO: Add Description**|
|principalId|Guid|**TODO: Add Description**|
|principalType|String|**TODO: Add Description**|
|resourceDisplayName|String|**TODO: Add Description**|
|resourceId|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_approleassignedto"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
Content-Type: application/json
Content-length: 461

{
  "@odata.type": "#Microsoft.DirectoryServices.appRoleAssignment",
  "appRoleId": "27bd2e88-2e88-27bd-882e-bd27882ebd27",
  "creationTimestamp": "2016-12-31T23:58:27.73127+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "0279f1dc-f1dc-0279-dcf1-7902dcf17902",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "95df367a-367a-95df-7a36-df957a36df95"
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
  "@odata.type": "#Microsoft.DirectoryServices.appRoleAssignment",
  "appRoleId": "27bd2e88-2e88-27bd-882e-bd27882ebd27",
  "creationTimestamp": "2016-12-31T23:58:27.73127+00:00",
  "id": "32a22532-2532-32a2-3225-a2323225a232",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "0279f1dc-f1dc-0279-dcf1-7902dcf17902",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "95df367a-367a-95df-7a36-df957a36df95"
}
```

