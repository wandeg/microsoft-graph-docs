---
title: "Get depOnboardingSetting"
description: "Read properties and relationships of the depOnboardingSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get depOnboardingSetting

Namespace: microsoft.graph

Read properties and relationships of the [depOnboardingSetting](../resources/deponboardingsetting.md) object.

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
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
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
If successful, this method returns a `200 OK` response code and [depOnboardingSetting](../resources/deponboardingsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_deponboardingsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 744

{
  "value": {
    "@odata.type": "#microsoft.graph.depOnboardingSetting",
    "id": "43c632e8-32e8-43c6-e832-c643e832c643",
    "appleIdentifier": "Apple Identifier value",
    "tokenExpirationDateTime": "2016-12-31T23:57:08.4624649+00:00",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:00:21.6152085+00:00",
    "lastSyncTriggeredDateTime": "2016-12-31T23:58:56.3554211+00:00",
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
}
```

