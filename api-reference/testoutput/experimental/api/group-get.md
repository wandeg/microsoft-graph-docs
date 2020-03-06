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
GET /me/joinedGroups/{groupId}
GET /users/{usersId}/joinedGroups/{groupId}
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
Content-Length: 2988

{
  "value": {
    "@odata.type": "#microsoft.graph.group",
    "id": "ad1a3cae-3cae-ad1a-ae3c-1aadae3c1aad",
    "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
    "assignedLabels": [
      {
        "@odata.type": "microsoft.graph.assignedLabel",
        "labelId": "Label Id value",
        "displayName": "Display Name value"
      }
    ],
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense",
        "disabledPlans": [
          "3c38c39b-c39b-3c38-9bc3-383c9bc3383c"
        ],
        "skuId": "25470e04-0e04-2547-040e-4725040e4725"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "groupTypes": [
      "Group Types value"
    ],
    "hasMembersWithLicenseErrors": true,
    "isAssignableToRole": true,
    "licenseProcessingState": {
      "@odata.type": "microsoft.graph.licenseProcessingState",
      "state": "State value"
    },
    "mail": "Mail value",
    "mailEnabled": true,
    "mailNickname": "Mail Nickname value",
    "mdmAppId": "Mdm App Id value",
    "membershipRule": "Membership Rule value",
    "membershipRuleProcessingState": "Membership Rule Processing State value",
    "onPremisesDomainName": "On Premises Domain Name value",
    "onPremisesLastSyncDateTime": "2016-12-31T23:58:33.0576521+03:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2016-12-31T23:56:49.154911+03:00"
      }
    ],
    "onPremisesSamAccountName": "On Premises Sam Account Name value",
    "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
    "onPremisesSyncEnabled": true,
    "preferredDataLocation": "Preferred Data Location value",
    "preferredLanguage": "Preferred Language value",
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "renewedDateTime": "2016-12-31T23:59:03.2446324+03:00",
    "resourceBehaviorOptions": [
      "Resource Behavior Options value"
    ],
    "resourceProvisioningOptions": [
      "Resource Provisioning Options value"
    ],
    "securityEnabled": true,
    "securityIdentifier": "Security Identifier value",
    "theme": "Theme value",
    "visibility": "Visibility value",
    "accessType": "String",
    "allowExternalSenders": true,
    "autoSubscribeNewMembers": true,
    "isFavorite": true,
    "isSubscribedByMail": true,
    "unseenCount": 11,
    "unseenConversationsCount": 8,
    "unseenMessagesCount": 3,
    "hideFromOutlookClients": true,
    "hideFromAddressLists": true,
    "isArchived": true
  }
}
```

