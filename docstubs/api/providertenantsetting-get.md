---
title: "Get providerTenantSetting"
description: "Read properties and relationships of the providerTenantSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get providerTenantSetting

Namespace: microsoft.graph

Read properties and relationships of the [providerTenantSetting](../resources/providertenantsetting.md) object.

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
GET /Security/providerTenantSettings/{providerTenantSettingId}
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
If successful, this method returns a `200 OK` response code and [providerTenantSetting](../resources/providertenantsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_providertenantsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/providerTenantSettings/{providerTenantSettingId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.providerTenantSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "value": {
    "@odata.type": "#microsoft.graph.providerTenantSetting",
    "id": "9a3775c3-75c3-9a37-c375-379ac375379a",
    "azureTenantId": "Azure Tenant Id value",
    "enabled": true,
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
    "provider": "Provider value",
    "vendor": "Vendor value"
  }
}
```

