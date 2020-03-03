---
title: "List groups"
description: "List properties and relationships of the group objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groups

Namespace: microsoft.graph

List properties and relationships of the [group](../resources/group.md) objects.

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
GET /groups
GET /me/joinedGroups
GET /users/{usersId}/joinedGroups
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
GET https://graph.microsoft.com/localtest/groups
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
Content-Length: 3162

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "2c3bc02c-c02c-2c3b-2cc0-3b2c2cc03b2c",
      "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
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
            "d28f3feb-3feb-d28f-eb3f-8fd2eb3f8fd2"
          ],
          "skuId": "766f47e4-47e4-766f-e447-6f76e4476f76"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:58:26.0302388+03:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2017-01-01T00:00:02.4393137+03:00"
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
      "renewedDateTime": "2017-01-01T00:02:09.3684079+03:00",
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
  ]
}
```

