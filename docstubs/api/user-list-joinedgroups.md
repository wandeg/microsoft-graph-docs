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
GET /users/{usersId}/joinedGroups
GET /invitations/{invitationsId}/invitedUser/joinedGroups
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
GET https://graph.microsoft.com/beta/users/{usersId}/joinedGroups
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
      "id": "33c0d48e-d48e-33c0-8ed4-c0338ed4c033",
      "deletedDateTime": "2017-01-01T00:03:11.3808645+03:00",
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
            "eba74958-4958-eba7-5849-a7eb5849a7eb"
          ],
          "skuId": "6aa85ab4-5ab4-6aa8-b45a-a86ab45aa86a"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:00:27.9270493+03:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:01:21.8025226+03:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2017-01-01T00:02:14.8347655+03:00"
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
      "renewedDateTime": "2016-12-31T23:59:08.8877336+03:00",
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

