---
title: "List editionUpgradeConfigurations"
description: "List properties and relationships of the editionUpgradeConfiguration objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List editionUpgradeConfigurations

Namespace: microsoft.graph

List properties and relationships of the [editionUpgradeConfiguration](../resources/editionupgradeconfiguration.md) objects.

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
GET ** Collection URI for microsoft.graph.editionUpgradeConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/editionupgradeconfiguration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_editionupgradeconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.editionUpgradeConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.editionupgradeconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
      "id": "0b860b22-0b22-0b86-220b-860b220b860b",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "licenseType": "String",
      "targetEdition": "String",
      "license": "License value",
      "productKey": "Product Key value"
    }
  ]
}
```

