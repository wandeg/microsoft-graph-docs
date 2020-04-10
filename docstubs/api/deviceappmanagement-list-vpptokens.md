---
title: "List vppTokens"
description: "Get the vppTokens from the vppTokens navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List vppTokens

Namespace: microsoft.graph

Get the vppTokens from the vppTokens navigation property.

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
GET /deviceAppManagement/vppTokens
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/vpptoken.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_vpptoken"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.vpptoken)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1257

{
  "value": [
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
  ]
}
```

