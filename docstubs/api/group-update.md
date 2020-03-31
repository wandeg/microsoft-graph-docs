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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_group"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}
Content-type: application/json
Content-length: 2701

{
  "@odata.type": "#microsoft.graph.group",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2809

{
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
```

