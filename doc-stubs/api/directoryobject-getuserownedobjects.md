---
title: "directoryObject: getUserOwnedObjects"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getUserOwnedObjects
Namespace: microsoft.graph

**TODO: Add Description**

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
POST /me/memberOf/getUserOwnedObjects
POST /me/ownedDevices/getUserOwnedObjects
POST /me/ownedObjects/getUserOwnedObjects
POST /directoryObjects/getUserOwnedObjects
POST /me/directReports/getUserOwnedObjects
POST /me/createdObjects/getUserOwnedObjects
POST /stsPolicy/appliesTo/getUserOwnedObjects
POST /me/registeredDevices/getUserOwnedObjects
POST /me/transitiveMemberOf/getUserOwnedObjects
POST /directory/deletedItems/getUserOwnedObjects
POST /groups/{groupsId}/owners/getUserOwnedObjects
POST /users/{usersId}/memberOf/getUserOwnedObjects
POST /groups/{groupsId}/members/getUserOwnedObjects
POST /groups/{groupsId}/memberOf/getUserOwnedObjects
POST /devices/{devicesId}/memberOf/getUserOwnedObjects
POST /users/{usersId}/ownedDevices/getUserOwnedObjects
POST /users/{usersId}/ownedObjects/getUserOwnedObjects
POST /users/{usersId}/directReports/getUserOwnedObjects
POST /contacts/{contactsId}/memberOf/getUserOwnedObjects
POST /users/{usersId}/createdObjects/getUserOwnedObjects
POST /users/{usersId}/registeredDevices/getUserOwnedObjects
POST /users/{usersId}/transitiveMemberOf/getUserOwnedObjects
POST /contacts/{contactsId}/directReports/getUserOwnedObjects
POST /devices/{devicesId}/registeredUsers/getUserOwnedObjects
POST /groups/{groupsId}/transitiveMembers/getUserOwnedObjects
POST /applications/{applicationsId}/owners/getUserOwnedObjects
POST /devices/{devicesId}/registeredOwners/getUserOwnedObjects
POST /groups/{groupsId}/transitiveMemberOf/getUserOwnedObjects
POST /devices/{devicesId}/transitiveMemberOf/getUserOwnedObjects
POST /contacts/{contactsId}/transitiveMemberOf/getUserOwnedObjects
POST /domains/{domainsId}/domainNameReferences/getUserOwnedObjects
POST /directoryRoles/{directoryRolesId}/members/getUserOwnedObjects
POST /groups/{groupsId}/membersWithLicenseErrors/getUserOwnedObjects
POST /servicePrincipals/{servicePrincipalsId}/owners/getUserOwnedObjects
POST /servicePrincipals/{servicePrincipalsId}/memberOf/getUserOwnedObjects
POST /administrativeUnits/{administrativeUnitsId}/members/getUserOwnedObjects
POST /servicePrincipals/{servicePrincipalsId}/ownedObjects/getUserOwnedObjects
POST /servicePrincipals/{servicePrincipalsId}/createdObjects/getUserOwnedObjects
POST /servicePrincipals/{servicePrincipalsId}/transitiveMemberOf/getUserOwnedObjects
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|userId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "directoryobject_getuserownedobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/memberOf/getUserOwnedObjects

Content-Type: application/json
Content-length: 47

{
  "userId": "String",
  "type": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)"
  }
}
```

