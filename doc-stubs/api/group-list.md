---
title: "List groups"
description: "Get a list of the group objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
|Authorization|Bearer {token}. Required.|

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
GET https://graph.microsoft.com/v1.0/groups
```


### Response
**Note:** The response object shown here might be shortened for readability.
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
      "id": "8cdd3c04-3c04-8cdd-043c-dd8c043cdd8c",
      "deletedDateTime": "String (timestamp)",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "classification": "String",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "hasMembersWithLicenseErrors": "Boolean",
      "groupTypes": [
        "String"
      ],
      "licenseProcessingState": {
        "@odata.type": "microsoft.graph.licenseProcessingState"
      },
      "mail": "String",
      "mailEnabled": "Boolean",
      "mailNickname": "String",
      "onPremisesDomainName": "String",
      "onPremisesLastSyncDateTime": "String (timestamp)",
      "onPremisesNetBiosName": "String",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError"
        }
      ],
      "onPremisesSamAccountName": "String",
      "onPremisesSecurityIdentifier": "String",
      "onPremisesSyncEnabled": "Boolean",
      "preferredDataLocation": "String",
      "proxyAddresses": [
        "String"
      ],
      "renewedDateTime": "String (timestamp)",
      "securityEnabled": "Boolean",
      "securityIdentifier": "String",
      "visibility": "String",
      "allowExternalSenders": "Boolean",
      "autoSubscribeNewMembers": "Boolean",
      "isSubscribedByMail": "Boolean",
      "unseenCount": "Integer",
      "hideFromOutlookClients": "Boolean",
      "hideFromAddressLists": "Boolean",
      "isArchived": "Boolean"
    }
  ]
}
```

