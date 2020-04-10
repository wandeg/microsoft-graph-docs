---
title: "Add vppTokens"
description: "Add vppTokens by posting to the vppTokens collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add vppTokens

Namespace: microsoft.graph

Add vppTokens by posting to the vppTokens collection.

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
POST /deviceAppManagement/vppTokens/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
Content-type: application/json
Content-length: 995

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "lastSyncDateTime": "2016-12-31T23:57:45.5058522+00:00",
  "token": "Token value",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "String",
      "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
      "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00"
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vpptoken"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1108

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9f8f5285-5285-9f8f-8552-8f9f85528f9f",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "lastSyncDateTime": "2016-12-31T23:57:45.5058522+00:00",
  "token": "Token value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "String",
      "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
      "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00"
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

