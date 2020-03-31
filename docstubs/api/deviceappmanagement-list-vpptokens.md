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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_vpptoken"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  ]
}
```

