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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
POST https://graph.microsoft.com/v1.0/groups/{groupsId}/assignLicense

Content-Type: application/json
Content-length: 140

{
  "addLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "removeLicenses": [
    "Guid"
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
    "id": "String (identifier)",
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
}
```

