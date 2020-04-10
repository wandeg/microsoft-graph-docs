---
title: "importedDeviceIdentity: searchExistingIdentities"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# searchExistingIdentities

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
POST /deviceManagement/importedDeviceIdentities/searchExistingIdentities
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



## Response
If successful, this action returns a `200 OK` response code and a [importedDeviceIdentity](../resources/importeddeviceidentity.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "importeddeviceidentity_searchexistingidentities"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/searchExistingIdentities

Content-type: application/json
Content-length: 599

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
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.importeddeviceidentity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 580

{
  "value": [
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
  ]
}
```

