---
title: "group: assignLicense"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# assignLicense

Namespace: Microsoft.DirectoryServices

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
|addLicenses|[assignedLicense](../resources/microsoft.directoryservices-assignedlicense.md) collection|**TODO: Add Description**|
|removeLicenses|Guid collection|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [group](../resources/microsoft.directoryservices-group.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}
-->
``` http
POST https://graph.microsoft.com/changelog/groups/{groupsId}/assignLicense

Content-Type: application/json
Content-length: 184

{
  "addLicenses": [
    {
      "@odata.type": "Microsoft.DirectoryServices.assignedLicense"
    }
  ],
  "removeLicenses": [
    "5cae58da-58da-5cae-da58-ae5cda58ae5c"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.group"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.group",
    "id": "468b7611-7611-468b-1176-8b4611768b46",
    "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
    "assignedLabels": [
      {
        "@odata.type": "Microsoft.DirectoryServices.assignedLabel"
      }
    ],
    "assignedLicenses": [
      {
        "@odata.type": "Microsoft.DirectoryServices.assignedLicense"
      }
    ],
    "classification": "Classification value",
    "createdDateTime": "2017-01-01T00:03:17.7218452+00:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "groupTypes": [
      "Group Types value"
    ],
    "hasMembersWithLicenseErrors": true,
    "isAssignableToRole": true,
    "licenseProcessingState": {
      "@odata.type": "Microsoft.DirectoryServices.licenseProcessingState"
    },
    "mail": "Mail value",
    "mailEnabled": true,
    "mailNickname": "Mail Nickname value",
    "mdmAppId": "Mdm App Id value",
    "membershipRule": "Membership Rule value",
    "membershipRuleProcessingState": "Membership Rule Processing State value",
    "onPremisesDomainName": "On Premises Domain Name value",
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
    "onPremisesNetBiosName": "On Premises Net Bios Name value",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError"
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
    "renewedDateTime": "2016-12-31T23:59:27.0216848+00:00",
    "resourceBehaviorOptions": [
      "Resource Behavior Options value"
    ],
    "resourceProvisioningOptions": [
      "Resource Provisioning Options value"
    ],
    "securityEnabled": true,
    "securityIdentifier": "Security Identifier value",
    "theme": "Theme value",
    "visibility": "Visibility value"
  }
}
```

