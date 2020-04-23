---
title: "List mobileAppConfigurations"
description: "Get the managedDeviceMobileAppConfigurations from the mobileAppConfigurations navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mobileAppConfigurations

Namespace: microsoft.graph

Get the managedDeviceMobileAppConfigurations from the mobileAppConfigurations navigation property.

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
GET /deviceAppManagement/mobileAppConfigurations
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
If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_manageddevicemobileappconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddevicemobileappconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
      "id": "c20691f6-91f6-c206-f691-06c2f69106c2",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```

