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
|Name|Description|
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
GET https://graph.microsoft.com/beta/groups/{groupsId}
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
    "id": "fd5b121e-121e-fd5b-1e12-5bfd1e125bfd",
    "deletedDateTime": "2016-12-31T23:56:41.707717+03:00",
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
          "44adad82-ad82-44ad-82ad-ad4482adad44"
        ],
        "skuId": "23cc04fd-04fd-23cc-fd04-cc23fd04cc23"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
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
    "onPremisesLastSyncDateTime": "2017-01-01T00:03:26.0023027+03:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2017-01-01T00:00:57.1452249+03:00"
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
    "renewedDateTime": "2017-01-01T00:00:21.6222922+03:00",
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

