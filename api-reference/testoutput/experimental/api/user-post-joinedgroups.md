---
title: "Add joinedGroups"
description: "Add joinedGroups by posting to the joinedGroups collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add joinedGroups

Add joinedGroups by posting to the joinedGroups collection.

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
POST /me/joinedGroups/$ref
POST /users/{usersId}/joinedGroups/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the group object.

The following table shows the properties that are required when you create the group.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|assignedLabels|[assignedLabel](../resources/assignedLabel.md) collection||
|assignedLicenses|[assignedLicense](../resources/assignedLicense.md) collection||
|classification|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|groupTypes|String collection||
|hasMembersWithLicenseErrors|Boolean||
|isAssignableToRole|Boolean||
|licenseProcessingState|[licenseProcessingState](../resources/licenseProcessingState.md)||
|mail|String||
|mailEnabled|Boolean||
|mailNickname|String||
|mdmAppId|String||
|membershipRule|String||
|membershipRuleProcessingState|String||
|onPremisesDomainName|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesNetBiosName|String||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onPremisesProvisioningError.md) collection||
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
|accessType|Enumeration|. Possible values are: `none`, `private`, `secret`, `public`.|
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
If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/joinedGroups
Content-type: application/json
Content-length: 2702

{
  "@odata.type": "#microsoft.graph.group",
  "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
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
        "018663cc-63cc-0186-cc63-8601cc638601"
      ],
      "skuId": "57435096-5096-5743-9650-435796504357"
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
  "onPremisesLastSyncDateTime": "2016-12-31T23:59:32.0778154+03:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:01:54.8756248+03:00"
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
  "renewedDateTime": "2016-12-31T23:59:56.7748726+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2810

{
  "@odata.type": "#microsoft.graph.group",
  "id": "a2a4952c-952c-a2a4-2c95-a4a22c95a4a2",
  "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
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
        "018663cc-63cc-0186-cc63-8601cc638601"
      ],
      "skuId": "57435096-5096-5743-9650-435796504357"
    }
  ],
  "classification": "Classification value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
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
  "onPremisesLastSyncDateTime": "2016-12-31T23:59:32.0778154+03:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:01:54.8756248+03:00"
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
  "renewedDateTime": "2016-12-31T23:59:56.7748726+03:00",
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

