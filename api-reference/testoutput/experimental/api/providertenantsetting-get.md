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

## HTTP Request
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
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [providerTenantSetting](../resources/providertenantsetting.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_providertenantsetting"
}
-->
``` http
GET https://graph.microsoft.com/localtest/Security/providerTenantSettings/{providerTenantSettingId}
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
    "id": "74e785a2-85a2-74e7-a285-e774a285e774",
    "azureTenantId": "Azure Tenant Id value",
    "enabled": true,
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
    "provider": "Provider value",
    "vendor": "Vendor value"
  }
}
```

