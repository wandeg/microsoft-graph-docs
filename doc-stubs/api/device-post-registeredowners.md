---
title: "Add registeredOwners"
description: "Add registeredOwners by posting to the registeredOwners collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add registeredOwners
Namespace: microsoft.graph

Add registeredOwners by posting to the registeredOwners collection.

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
POST /me/memberOf/$ref
POST /me/ownedDevices/$ref
POST /me/ownedObjects/$ref
POST /directoryObjects/$ref
POST /me/directReports/$ref
POST /me/createdObjects/$ref
POST /stsPolicy/appliesTo/$ref
POST /me/registeredDevices/$ref
POST /me/transitiveMemberOf/$ref
POST /directory/deletedItems/$ref
POST /groups/{groupsId}/owners/$ref
POST /users/{usersId}/memberOf/$ref
POST /groups/{groupsId}/members/$ref
POST /groups/{groupsId}/memberOf/$ref
POST /devices/{devicesId}/memberOf/$ref
POST /users/{usersId}/ownedDevices/$ref
POST /users/{usersId}/ownedObjects/$ref
POST /users/{usersId}/directReports/$ref
POST /contacts/{contactsId}/memberOf/$ref
POST /users/{usersId}/createdObjects/$ref
POST /users/{usersId}/registeredDevices/$ref
POST /users/{usersId}/transitiveMemberOf/$ref
POST /contacts/{contactsId}/directReports/$ref
POST /devices/{devicesId}/registeredUsers/$ref
POST /groups/{groupsId}/transitiveMembers/$ref
POST /applications/{applicationsId}/owners/$ref
POST /devices/{devicesId}/registeredOwners/$ref
POST /groups/{groupsId}/transitiveMemberOf/$ref
POST /devices/{devicesId}/transitiveMemberOf/$ref
POST /contacts/{contactsId}/transitiveMemberOf/$ref
POST /domains/{domainsId}/domainNameReferences/$ref
POST /directoryRoles/{directoryRolesId}/members/$ref
POST /groups/{groupsId}/membersWithLicenseErrors/$ref
POST /servicePrincipals/{servicePrincipalsId}/owners/$ref
POST /servicePrincipals/{servicePrincipalsId}/memberOf/$ref
POST /administrativeUnits/{administrativeUnitsId}/members/$ref
POST /servicePrincipals/{servicePrincipalsId}/ownedObjects/$ref
POST /servicePrincipals/{servicePrincipalsId}/createdObjects/$ref
POST /servicePrincipals/{servicePrincipalsId}/transitiveMemberOf/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/memberOf/$ref
Content-Type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "String (timestamp)"
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
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "be332a57-2a57-be33-572a-33be572a33be",
  "deletedDateTime": "String (timestamp)"
}
```

