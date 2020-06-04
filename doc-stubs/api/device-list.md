---
title: "List devices"
description: "Get a list of the device objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List devices
Namespace: microsoft.graph

Get a list of the [device](../resources/device.md) objects and their properties.

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
GET /devices
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [device](../resources/device.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.device)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.device",
      "id": "1c675635-5635-1c67-3556-671c3556671c",
      "deletedDateTime": "String (timestamp)",
      "accountEnabled": "Boolean",
      "alternativeSecurityIds": [
        {
          "@odata.type": "microsoft.graph.alternativeSecurityId"
        }
      ],
      "approximateLastSignInDateTime": "String (timestamp)",
      "complianceExpirationDateTime": "String (timestamp)",
      "deviceId": "String",
      "deviceMetadata": "String",
      "deviceVersion": "Integer",
      "displayName": "String",
      "extensionAttributes": {
        "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
      },
      "isCompliant": "Boolean",
      "isManaged": "Boolean",
      "onPremisesLastSyncDateTime": "String (timestamp)",
      "onPremisesSyncEnabled": "Boolean",
      "operatingSystem": "String",
      "operatingSystemVersion": "String",
      "physicalIds": [
        "String"
      ],
      "profileType": "String",
      "systemLabels": [
        "String"
      ],
      "trustType": "String"
    }
  ]
}
```

