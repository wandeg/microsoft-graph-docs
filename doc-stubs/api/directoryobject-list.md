---
title: "List directoryObjects"
description: "Get a list of the directoryObject objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List directoryObjects

Namespace: microsoft.graph

Get a list of the [directoryObject](../resources/directoryobject.md) objects and their properties.

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
GET /directoryObjects
GET /stsPolicy/appliesTo
GET /directory/deletedItems
GET /groups/{groupsId}/owners
GET /groups/{groupsId}/members
GET /groups/{groupsId}/memberOf
GET /devices/{devicesId}/memberOf
GET /contacts/{contactsId}/memberOf
GET /groups/{groupsId}/acceptedSenders
GET /groups/{groupsId}/rejectedSenders
GET /contacts/{contactsId}/directReports
GET /devices/{devicesId}/registeredUsers
GET /groups/{groupsId}/transitiveMembers
GET /devices/{devicesId}/registeredOwners
GET /groups/{groupsId}/transitiveMemberOf
GET /devices/{devicesId}/transitiveMemberOf
GET /contacts/{contactsId}/transitiveMemberOf
GET /domains/{domainsId}/domainNameReferences
GET /directoryRoles/{directoryRolesId}/members
GET /groups/{groupsId}/membersWithLicenseErrors
GET /servicePrincipals/{servicePrincipalsId}/owners
GET /servicePrincipals/{servicePrincipalsId}/memberOf
GET /servicePrincipals/{servicePrincipalsId}/ownedObjects
GET /servicePrincipals/{servicePrincipalsId}/createdObjects
GET /servicePrincipals/{servicePrincipalsId}/transitiveMemberOf
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/directoryObjects
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryobject)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryObject",
      "id": "c394496f-496f-c394-6f49-94c36f4994c3",
      "deletedDateTime": "String (timestamp)"
    }
  ]
}
```

