---
title: "List joinedGroups"
description: "Get the groups from the joinedGroups navigation property."
author: ""
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
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups
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
Content-Length: 3160

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "5d164841-4841-5d16-4148-165d4148165d",
      "deletedDateTime": "2017-01-01T00:03:25.5057888+00:00",
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
            "9cad76b9-76b9-9cad-b976-ad9cb976ad9c"
          ],
          "skuId": "7ac02db4-2db4-7ac0-b42d-c07ab42dc07a"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:00:49.2255493+00:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:00:18.668834+00:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:56:25.21852+00:00"
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
      "renewedDateTime": "2017-01-01T00:01:40.9466213+00:00",
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

