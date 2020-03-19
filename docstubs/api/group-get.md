---
title: "Get group"
description: "Read properties and relationships of the group object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get group

Namespace: microsoft.graph

Read properties and relationships of the [group](../resources/group.md) object.

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
GET /groups/{groupsId}
GET /me/joinedTeams/{groupId}
GET /users/{usersId}/joinedTeams/{groupId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2150

{
  "value": {
    "@odata.type": "#microsoft.graph.group",
    "id": "ad0e53b6-53b6-ad0e-b653-0eadb6530ead",
    "deletedDateTime": "2017-01-01T00:00:51.5607674+03:00",
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense",
        "disabledPlans": [
          "e4badb69-db69-e4ba-69db-bae469dbbae4"
        ],
        "skuId": "d46c0125-0125-d46c-2501-6cd425016cd4"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2017-01-01T00:00:57.6286041+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "hasMembersWithLicenseErrors": true,
    "groupTypes": [
      "Group Types value"
    ],
    "licenseProcessingState": {
      "@odata.type": "microsoft.graph.licenseProcessingState",
      "state": "State value"
    },
    "mail": "Mail value",
    "mailEnabled": true,
    "mailNickname": "Mail Nickname value",
    "onPremisesDomainName": "On Premises Domain Name value",
    "onPremisesLastSyncDateTime": "2017-01-01T00:02:11.1510411+03:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2016-12-31T23:59:35.2221313+03:00"
      }
    ],
    "onPremisesSamAccountName": "On Premises Sam Account Name value",
    "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
    "onPremisesSyncEnabled": true,
    "preferredDataLocation": "Preferred Data Location value",
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "renewedDateTime": "2017-01-01T00:03:11.4286363+03:00",
    "securityEnabled": true,
    "securityIdentifier": "Security Identifier value",
    "visibility": "Visibility value",
    "allowExternalSenders": true,
    "autoSubscribeNewMembers": true,
    "isSubscribedByMail": true,
    "unseenCount": 11,
    "isArchived": true
  }
}
```

