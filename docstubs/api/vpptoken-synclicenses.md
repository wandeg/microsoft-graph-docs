---
title: "syncLicenses"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# syncLicenses

Namespace: microsoft.graph



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
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [vppToken](../resources/vpptoken.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "vpptoken_synclicenses"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vpptoken"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 975

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "1e23ddf8-ddf8-1e23-f8dd-231ef8dd231e",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "String",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:21.3858094+03:00",
    "lastSyncDateTime": "2017-01-01T00:02:12.9318449+03:00",
    "token": "Token value",
    "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
    "state": "String",
    "tokenActionResults": [
      {
        "@odata.type": "microsoft.graph.vppTokenActionResult"
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
}
```

