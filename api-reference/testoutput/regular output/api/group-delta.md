---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /groups/delta
GET /me/joinedTeams/delta
GET /users/{usersId}/joinedTeams/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [group](../resources/group.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "group_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/delta
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
Content-Length: 1874

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "0a7bb131-b131-0a7b-31b1-7b0a31b17b0a",
      "deletedDateTime": "2017-01-01T00:02:06.0464622+03:00",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:01:25.3917672+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "hasMembersWithLicenseErrors": true,
      "groupTypes": [
        "Group Types value"
      ],
      "licenseProcessingState": {
        "@odata.type": "microsoft.graph.licenseProcessingState"
      },
      "mail": "Mail value",
      "mailEnabled": true,
      "mailNickname": "Mail Nickname value",
      "onPremisesDomainName": "On Premises Domain Name value",
      "onPremisesLastSyncDateTime": "2017-01-01T00:00:16.9182164+03:00",
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
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "renewedDateTime": "2016-12-31T23:57:03.7606659+03:00",
      "securityEnabled": true,
      "securityIdentifier": "Security Identifier value",
      "visibility": "Visibility value",
      "allowExternalSenders": true,
      "autoSubscribeNewMembers": true,
      "isSubscribedByMail": true,
      "unseenCount": 11,
      "isArchived": true
    }
  ]
}
```

