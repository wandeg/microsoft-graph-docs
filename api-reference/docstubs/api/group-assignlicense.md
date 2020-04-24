---
title: "group: assignLicense"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# assignLicense

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /groups/{groupsId}/assignLicense
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|removeLicenses|Guid collection|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [group](../resources/group.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/assignLicense

Content-Type: application/json
Content-length: 172

{
  "addLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "removeLicenses": [
    "be300029-0029-be30-2900-30be290030be"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.group",
    "id": "b6d00a80-0a80-b6d0-800a-d0b6800ad0b6",
    "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
    "assignedLabels": [
      {
        "@odata.type": "microsoft.graph.assignedLabel"
      }
    ],
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "groupTypes": [
      "Group Types value"
    ],
    "hasMembersWithLicenseErrors": true,
    "isAssignableToRole": true,
    "licenseProcessingState": {
      "@odata.type": "microsoft.graph.licenseProcessingState"
    },
    "mail": "Mail value",
    "mailEnabled": true,
    "mailNickname": "Mail Nickname value",
    "mdmAppId": "Mdm App Id value",
    "membershipRule": "Membership Rule value",
    "membershipRuleProcessingState": "Membership Rule Processing State value",
    "onPremisesDomainName": "On Premises Domain Name value",
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError"
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
    "renewedDateTime": "2016-12-31T23:57:46.0334281+03:00",
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

