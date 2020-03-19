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
Content-Length: 2149

{
  "value": {
    "@odata.type": "#microsoft.graph.group",
    "id": "92632a3c-2a3c-9263-3c2a-63923c2a6392",
    "deletedDateTime": "2017-01-01T00:03:19.6121707+03:00",
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense",
        "disabledPlans": [
          "045d3503-3503-045d-0335-5d0403355d04"
        ],
        "skuId": "a80ed027-d027-a80e-27d0-0ea827d00ea8"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2016-12-31T23:58:36.6060207+03:00",
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
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:10.365865+03:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2016-12-31T23:58:36.5082341+03:00"
      }
    ],
    "onPremisesSamAccountName": "On Premises Sam Account Name value",
    "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
    "onPremisesSyncEnabled": true,
    "preferredDataLocation": "Preferred Data Location value",
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "renewedDateTime": "2016-12-31T23:58:05.6533023+03:00",
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

