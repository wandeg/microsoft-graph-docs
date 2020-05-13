---
title: "Create directoryObject"
description: "Create a new directoryObject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directoryObject

Namespace: microsoft.graph

Create a new [directoryObject](../resources/directoryobject.md) object.

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
POST /directoryObjects
POST /stsPolicy/appliesTo
POST /directory/deletedItems
POST /groups/{groupsId}/owners
POST /groups/{groupsId}/members
POST /groups/{groupsId}/memberOf
POST /devices/{devicesId}/memberOf
POST /contacts/{contactsId}/memberOf
POST /groups/{groupsId}/acceptedSenders
POST /groups/{groupsId}/rejectedSenders
POST /contacts/{contactsId}/directReports
POST /devices/{devicesId}/registeredUsers
POST /groups/{groupsId}/transitiveMembers
POST /devices/{devicesId}/registeredOwners
POST /groups/{groupsId}/transitiveMemberOf
POST /devices/{devicesId}/transitiveMemberOf
POST /contacts/{contactsId}/transitiveMemberOf
POST /domains/{domainsId}/domainNameReferences
POST /directoryRoles/{directoryRolesId}/members
POST /groups/{groupsId}/membersWithLicenseErrors
POST /servicePrincipals/{servicePrincipalsId}/owners
POST /servicePrincipals/{servicePrincipalsId}/memberOf
POST /servicePrincipals/{servicePrincipalsId}/ownedObjects
POST /servicePrincipals/{servicePrincipalsId}/createdObjects
POST /servicePrincipals/{servicePrincipalsId}/transitiveMemberOf
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

If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryobjects"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects
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
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "2cca027e-027e-2cca-7e02-ca2c7e02ca2c",
  "deletedDateTime": "String (timestamp)"
}
```

