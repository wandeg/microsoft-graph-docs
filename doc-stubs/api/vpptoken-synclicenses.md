---
title: "vppToken: syncLicenses"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# syncLicenses

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
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `200 OK` response code and a [vppToken](../resources/vpptoken.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "vpptoken_synclicenses"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
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
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "String (identifier)",
    "organizationName": "String",
    "vppTokenAccountType": "String",
    "appleId": "String",
    "expirationDateTime": "String (timestamp)",
    "lastSyncDateTime": "String (timestamp)",
    "token": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "state": "String",
    "tokenActionResults": [
      {
        "@odata.type": "microsoft.graph.vppTokenActionResult"
      }
    ],
    "lastSyncStatus": "String",
    "automaticallyUpdateApps": "Boolean",
    "countryOrRegion": "String",
    "dataSharingConsentGranted": "Boolean",
    "displayName": "String",
    "locationName": "String",
    "claimTokenManagementFromExternalMdm": "Boolean",
    "roleScopeTagIds": [
      "String"
    ]
  }
}
```

