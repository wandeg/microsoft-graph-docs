---
title: "List joinedTeams"
description: "Get the groups from the joinedTeams navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List joinedTeams

Namespace: microsoft.graph

Get the groups from the joinedTeams navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/joinedTeams
GET /users/{usersId}/joinedTeams
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cd782a07-2a07-cd78-072a-78cd072a78cd",
      "deletedDateTime": "2017-01-01T00:02:42.9789072+03:00",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "a275d3dd-d3dd-a275-ddd3-75a2ddd375a2"
          ],
          "skuId": "c6055fc8-5fc8-c605-c85f-05c6c85f05c6"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:58:15.8013979+03:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:58:37.7821236+03:00"
        }
      ],
      "onPremisesSamAccountName": "On Premises Sam Account Name value",
      "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
      "onPremisesSyncEnabled": true,
      "preferredDataLocation": "Preferred Data Location value",
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "renewedDateTime": "2017-01-01T00:00:46.4465399+03:00",
      "securityEnabled": true,
      "securityIdentifier": "Security Identifier value",
      "visibility": "Visibility value",
      "allowExternalSenders": true,
      "autoSubscribeNewMembers": true,
      "isSubscribedByMail": true,
      "unseenCount": 11,
      "isArchived": true
    }
  ]
}
```

