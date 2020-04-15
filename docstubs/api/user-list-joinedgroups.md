---
title: "List joinedGroups"
description: "Get the groups from the joinedGroups navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List joinedGroups

Namespace: microsoft.graph

Get the groups from the joinedGroups navigation property.

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
GET /me/joinedGroups
GET /users/{usersId}/joinedGroups
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "7e5ebbe9-bbe9-7e5e-e9bb-5e7ee9bb5e7e",
      "deletedDateTime": "2016-12-31T23:58:28.3197258+03:00",
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
            "3f6680db-80db-3f66-db80-663fdb80663f"
          ],
          "skuId": "9f7a5a26-5a26-9f7a-265a-7a9f265a7a9f"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:00:27.4994223+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:59:16.9945393+03:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2017-01-01T00:00:34.639927+03:00"
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
      "renewedDateTime": "2017-01-01T00:02:14.8329799+03:00",
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

