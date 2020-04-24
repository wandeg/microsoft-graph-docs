---
title: "Create vppTokens"
description: "Create a new vppTokens object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create vppTokens

Namespace: microsoft.graph

Create a new vppTokens object.

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
POST /deviceAppManagement/vppTokens
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [vppToken](../resources/vpptoken.md) object.

The following table shows the properties that are required when you create the [vppToken](../resources/vpptoken.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|organizationName|String|The organization associated with the Apple Volume Purchase Program Token|
|vppTokenAccountType|vppTokenAccountType|The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. Possible values are: `business`, `education`. Possible values are: `business`, `education`.|
|appleId|String|The apple Id associated with the given Apple Volume Purchase Program Token.|
|expirationDateTime|DateTimeOffset|The expiration date time of the Apple Volume Purchase Program Token.|
|lastSyncDateTime|DateTimeOffset|The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.|
|token|String|The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Last modification date time associated with the Apple Volume Purchase Program Token.|
|state|vppTokenState|Current state of the Apple Volume Purchase Program Token. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|[vppTokenActionResult](../resources/vpptokenactionresult.md) collection|The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.|
|lastSyncStatus|vppTokenSyncStatus|Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token. Possible values are: `none`, `inProgress`, `completed`, `failed`. Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Whether or not apps for the VPP token will be automatically updated.|
|countryOrRegion|String|Whether or not apps for the VPP token will be automatically updated.|
|dataSharingConsentGranted|Boolean|Consent granted for data sharing with the Apple Volume Purchase Program.|
|displayName|String|An admin specified token friendly name.|
|locationName|String|Token location returned from Apple VPP.|
|claimTokenManagementFromExternalMdm|Boolean|Admin consent to allow claiming token management from external MDM.|
|roleScopeTagIds|String collection|Role Scope Tags IDs assigned to this entity.|



## Response
If successful, this method returns a `201 Created` response code and a [vppToken](../resources/vpptoken.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_vpptoken_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
Content-Type: application/json
Content-length: 994

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
  "token": "Token value",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "String",
      "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vpptoken"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "e07310af-10af-e073-af10-73e0af1073e0",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
  "token": "Token value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "String",
      "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

