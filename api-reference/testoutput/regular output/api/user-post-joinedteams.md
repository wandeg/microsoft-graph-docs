---
title: "Add joinedTeams"
description: "Add joinedTeams by posting to the joinedTeams collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add joinedTeams

Namespace: microsoft.graph

Add joinedTeams by posting to the joinedTeams collection.

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
POST /me/joinedTeams/$ref
POST /users/{usersId}/joinedTeams/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [group](../resources/group.md) object.

The following table shows the properties that are required when you create the [group](../resources/group.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|classification|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|hasMembersWithLicenseErrors|Boolean||
|groupTypes|String collection||
|licenseProcessingState|[licenseProcessingState](../resources/licenseprocessingstate.md)||
|mail|String||
|mailEnabled|Boolean||
|mailNickname|String||
|onPremisesDomainName|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesNetBiosName|String||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection||
|onPremisesSamAccountName|String||
|onPremisesSecurityIdentifier|String||
|onPremisesSyncEnabled|Boolean||
|preferredDataLocation|String||
|proxyAddresses|String collection||
|renewedDateTime|DateTimeOffset||
|securityEnabled|Boolean||
|securityIdentifier|String||
|visibility|String||
|allowExternalSenders|Boolean||
|autoSubscribeNewMembers|Boolean||
|isSubscribedByMail|Boolean||
|unseenCount|Int32||
|isArchived|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedTeams
Content-type: application/json
Content-length: 1913

{
  "@odata.type": "#microsoft.graph.group",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "964343ea-43ea-9643-ea43-4396ea434396"
      ],
      "skuId": "79ca07bb-07bb-79ca-bb07-ca79bb07ca79"
    }
  ],
  "classification": "Classification value",
  "description": "Description value",
  "displayName": "Display Name value",
  "hasMembersWithLicenseErrors": true,
  "groupTypes": [
    "Group Types value"
  ],
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState",
    "state": "State value"
  },
  "mail": "Mail value",
  "mailEnabled": true,
  "mailNickname": "Mail Nickname value",
  "onPremisesDomainName": "On Premises Domain Name value",
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:02.9589742+03:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:59:30.1342335+03:00"
    }
  ],
  "onPremisesSamAccountName": "On Premises Sam Account Name value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "Preferred Data Location value",
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "renewedDateTime": "2016-12-31T23:57:32.3555352+03:00",
  "securityEnabled": true,
  "securityIdentifier": "Security Identifier value",
  "visibility": "Visibility value",
  "allowExternalSenders": true,
  "autoSubscribeNewMembers": true,
  "isSubscribedByMail": true,
  "unseenCount": 11,
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
Content-Length: 2021

{
  "@odata.type": "#microsoft.graph.group",
  "id": "12dc0fee-0fee-12dc-ee0f-dc12ee0fdc12",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "964343ea-43ea-9643-ea43-4396ea434396"
      ],
      "skuId": "79ca07bb-07bb-79ca-bb07-ca79bb07ca79"
    }
  ],
  "classification": "Classification value",
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "hasMembersWithLicenseErrors": true,
  "groupTypes": [
    "Group Types value"
  ],
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState",
    "state": "State value"
  },
  "mail": "Mail value",
  "mailEnabled": true,
  "mailNickname": "Mail Nickname value",
  "onPremisesDomainName": "On Premises Domain Name value",
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:02.9589742+03:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:59:30.1342335+03:00"
    }
  ],
  "onPremisesSamAccountName": "On Premises Sam Account Name value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "Preferred Data Location value",
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "renewedDateTime": "2016-12-31T23:57:32.3555352+03:00",
  "securityEnabled": true,
  "securityIdentifier": "Security Identifier value",
  "visibility": "Visibility value",
  "allowExternalSenders": true,
  "autoSubscribeNewMembers": true,
  "isSubscribedByMail": true,
  "unseenCount": 11,
  "isArchived": true
}
```

