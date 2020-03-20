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
PATCH /me/joinedTeams/{groupId}
PATCH /users/{usersId}/joinedTeams/{groupId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
PATCH https://graph.microsoft.com/localtest/groups/{groupsId}
Content-type: application/json
Content-length: 1913

{
  "@odata.type": "#microsoft.graph.group",
  "deletedDateTime": "2016-12-31T23:57:46.8937102+00:00",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "6b73b825-b825-6b73-25b8-736b25b8736b"
      ],
      "skuId": "2e1281ae-81ae-2e12-ae81-122eae81122e"
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
  "onPremisesLastSyncDateTime": "2016-12-31T23:59:42.0239226+00:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:02:46.0147296+00:00"
    }
  ],
  "onPremisesSamAccountName": "On Premises Sam Account Name value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "Preferred Data Location value",
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "renewedDateTime": "2016-12-31T23:57:19.0396574+00:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2021

{
  "@odata.type": "#microsoft.graph.group",
  "id": "3d230c7e-0c7e-3d23-7e0c-233d7e0c233d",
  "deletedDateTime": "2016-12-31T23:57:46.8937102+00:00",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "6b73b825-b825-6b73-25b8-736b25b8736b"
      ],
      "skuId": "2e1281ae-81ae-2e12-ae81-122eae81122e"
    }
  ],
  "classification": "Classification value",
  "createdDateTime": "2017-01-01T00:02:48.1930499+00:00",
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
  "onPremisesLastSyncDateTime": "2016-12-31T23:59:42.0239226+00:00",
  "onPremisesNetBiosName": "On Premises Net Bios Name value",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:02:46.0147296+00:00"
    }
  ],
  "onPremisesSamAccountName": "On Premises Sam Account Name value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "Preferred Data Location value",
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "renewedDateTime": "2016-12-31T23:57:19.0396574+00:00",
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

