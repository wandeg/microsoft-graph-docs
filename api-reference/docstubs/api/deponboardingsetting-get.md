---
title: "Get depOnboardingSetting"
description: "Read the properties and relationships of a depOnboardingSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get depOnboardingSetting

Namespace: microsoft.graph

Read the properties and relationships of a [depOnboardingSetting](../resources/deponboardingsetting.md) object.

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
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [depOnboardingSetting](../resources/deponboardingsetting.md) object in the response body.

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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.depOnboardingSetting",
    "id": "2f2d4a1e-4a1e-2f2d-1e4a-2d2f1e4a2d2f",
    "appleIdentifier": "Apple Identifier value",
    "tokenExpirationDateTime": "2017-01-01T00:02:00.2078511+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:01:49.8221557+03:00",
    "lastSyncTriggeredDateTime": "2017-01-01T00:01:12.5172392+03:00",
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

