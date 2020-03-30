---
title: "List providerTenantSettings"
description: "Get the providerTenantSettings from the providerTenantSettings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List providerTenantSettings

Namespace: microsoft.graph

Get the providerTenantSettings from the providerTenantSettings navigation property.

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
GET /Security/providerTenantSettings
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
If successful, this method returns a `200 OK` response code and a collection of [providerTenantSetting](../resources/providertenantsetting.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_providertenantsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/providerTenantSettings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.providertenantsetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.providerTenantSetting",
      "id": "31bbb11d-b11d-31bb-1db1-bb311db1bb31",
      "azureTenantId": "Azure Tenant Id value",
      "enabled": true,
      "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00",
      "provider": "Provider value",
      "vendor": "Vendor value"
    }
  ]
}
```

