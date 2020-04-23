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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
    "id": "95fe7d28-7d28-95fe-287d-fe95287dfe95",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "String",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:58:13.22093+03:00",
    "lastSyncDateTime": "2017-01-01T00:03:21.3080262+03:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
    "state": "String",
    "lastSyncStatus": "String",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```

