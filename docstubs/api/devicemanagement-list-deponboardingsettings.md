---
title: "List depOnboardingSettings"
description: "Get the depOnboardingSettings from the depOnboardingSettings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List depOnboardingSettings

Namespace: microsoft.graph

Get the depOnboardingSettings from the depOnboardingSettings navigation property.

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
GET /deviceManagement/depOnboardingSettings
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
If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/deponboardingsetting.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deponboardingsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deponboardingsetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depOnboardingSetting",
      "id": "b0912aed-2aed-b091-ed2a-91b0ed2a91b0",
      "appleIdentifier": "Apple Identifier value",
      "tokenExpirationDateTime": "2017-01-01T00:00:36.9582138+00:00",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
      "lastSuccessfulSyncDateTime": "2017-01-01T00:01:58.6386615+00:00",
      "lastSyncTriggeredDateTime": "2017-01-01T00:02:01.5533664+00:00",
      "shareTokenWithSchoolDataSyncService": true,
      "lastSyncErrorCode": 1,
      "tokenType": "String",
      "tokenName": "Token Name value",
      "syncedDeviceCount": 1,
      "dataSharingConsentGranted": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```

