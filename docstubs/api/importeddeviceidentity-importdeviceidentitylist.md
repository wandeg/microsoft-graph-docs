---
title: "importedDeviceIdentity: importDeviceIdentityList"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# importDeviceIdentityList

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
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection||
|overwriteImportedDeviceIdentities|Boolean||



## Response
If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "importeddeviceidentity_importdeviceidentitylist"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 645

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "780fc647-c647-780f-47c6-0f7847c60f78",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "String",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "lastContactedDateTime": "2016-12-31T23:59:07.8428703+00:00",
      "description": "Description value",
      "enrollmentState": "String",
      "platform": "String"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.importeddeviceidentityresult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 609

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "ac6a16fe-16fe-ac6a-fe16-6aacfe166aac",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "String",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "lastContactedDateTime": "2016-12-31T23:59:07.8428703+00:00",
      "description": "Description value",
      "enrollmentState": "String",
      "platform": "String",
      "status": true
    }
  ]
}
```

