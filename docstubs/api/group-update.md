---
title: "Update group"
description: "Update the properties of a group object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update group

Namespace: microsoft.graph

Update the properties of a [group](../resources/group.md) object.

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
PATCH /groups/{groupsId}
PATCH /me/joinedGroups/{groupId}
PATCH /users/{usersId}/joinedGroups/{groupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [group](../resources/group.md) object.

The following table shows the properties that are required when you create the [group](../resources/group.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|assignedLabels|[assignedLabel](../resources/assignedlabel.md) collection||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|classification|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|groupTypes|String collection||
|hasMembersWithLicenseErrors|Boolean||
|isAssignableToRole|Boolean||
|licenseProcessingState|[licenseProcessingState](../resources/licenseprocessingstate.md)||
|mail|String||
|mailEnabled|Boolean||
|mailNickname|String||
|mdmAppId|String||
|membershipRule|String||
|membershipRuleProcessingState|String||
|onPremisesDomainName|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesNetBiosName|String||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection||
|onPremisesSamAccountName|String||
|onPremisesSecurityIdentifier|String||
|onPremisesSyncEnabled|Boolean||
|preferredDataLocation|String||
|preferredLanguage|String||
|proxyAddresses|String collection||
|renewedDateTime|DateTimeOffset||
|resourceBehaviorOptions|String collection||
|resourceProvisioningOptions|String collection||
|securityEnabled|Boolean||
|securityIdentifier|String||
|theme|String||
|visibility|String||
|accessType|Enumeration| Possible values are: `none`, `private`, `secret`, `public`.|
|allowExternalSenders|Boolean||
|autoSubscribeNewMembers|Boolean||
|isFavorite|Boolean||
|isSubscribedByMail|Boolean||
|unseenCount|Int32||
|unseenConversationsCount|Int32||
|unseenMessagesCount|Int32||
|hideFromOutlookClients|Boolean||
|hideFromAddressLists|Boolean||
|isArchived|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [group](../resources/group.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_group"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}
Content-type: application/json
Content-length: 2702

{
  "@odata.type": "#microsoft.graph.group",
  "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
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
        "360c11c0-11c0-360c-c011-0c36c0110c36"
      ],
      "skuId": "860ff1b8-f1b8-860f-b8f1-0f86b8f10f86"
    }
  ],
  "classification": "Classification value",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:02:42.7451887+00:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:58:59.9272029+00:00"
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
  "renewedDateTime": "2016-12-31T23:57:16.3202509+00:00",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2810

{
  "@odata.type": "#microsoft.graph.group",
  "id": "d02ae476-e476-d02a-76e4-2ad076e42ad0",
  "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
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
        "360c11c0-11c0-360c-c011-0c36c0110c36"
      ],
      "skuId": "860ff1b8-f1b8-860f-b8f1-0f86b8f10f86"
    }
  ],
  "classification": "Classification value",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:02:42.7451887+00:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:58:59.9272029+00:00"
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
  "renewedDateTime": "2016-12-31T23:57:16.3202509+00:00",
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
```

