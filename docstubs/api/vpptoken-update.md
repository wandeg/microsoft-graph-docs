---
title: "Update vppToken"
description: "Update the properties of a vppToken object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update vppToken

Namespace: microsoft.graph

Update the properties of a [vppToken](../resources/vpptoken.md) object.

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
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [vppToken](../resources/vpptoken.md) object.

The following table shows the properties that are required when you create the [vppToken](../resources/vpptoken.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|organizationName|String||
|vppTokenAccountType|Enumeration| Possible values are: `business`, `education`.|
|appleId|String||
|expirationDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|token|String||
|lastModifiedDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|[vppTokenActionResult](../resources/vpptokenactionresult.md) collection||
|lastSyncStatus|Enumeration| Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean||
|countryOrRegion|String||
|dataSharingConsentGranted|Boolean||
|displayName|String||
|locationName|String||
|claimTokenManagementFromExternalMdm|Boolean||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/vpptoken.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_vpptoken"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 995

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "lastSyncDateTime": "2017-01-01T00:03:05.8629729+03:00",
  "token": "Token value",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "String",
      "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:56:44.5564137+03:00"
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1108

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "77031fc0-1fc0-7703-c01f-0377c01f0377",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "lastSyncDateTime": "2017-01-01T00:03:05.8629729+03:00",
  "token": "Token value",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "String",
      "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:56:44.5564137+03:00"
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

