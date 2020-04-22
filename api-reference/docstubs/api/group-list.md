---
title: "List groups"
description: "Get a list of the group objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List groups

Namespace: microsoft.graph

Get a list of the [group](../resources/group.md) objects and their properties.

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
GET /groups
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
GET https://graph.microsoft.com/beta/groups
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
      "id": "ab2377d3-77d3-ab23-d377-23abd37723ab",
      "deletedDateTime": "2016-12-31T23:59:39.086137+00:00",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "03106d50-6d50-0310-506d-1003506d1003"
          ],
          "skuId": "d7fc8964-8964-d7fc-6489-fcd76489fcd7"
        }
      ],
      "classification": "Classification value",
      "createdDateTime": "2017-01-01T00:02:14.13292+00:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:01:21.5753431+00:00",
      "onPremisesNetBiosName": "On Premises Net Bios Name value",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:58:16.8919818+00:00"
        }
      ],
      "onPremisesSamAccountName": "On Premises Sam Account Name value",
      "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
      "onPremisesSyncEnabled": true,
      "preferredDataLocation": "Preferred Data Location value",
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "renewedDateTime": "2016-12-31T23:57:17.6749338+00:00",
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

