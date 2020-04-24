---
title: "Get providerTenantSetting"
description: "Read the properties and relationships of a providerTenantSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get providerTenantSetting

Namespace: microsoft.graph

Read the properties and relationships of a [providerTenantSetting](../resources/providertenantsetting.md) object.

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
GET /Security/providerTenantSettings/{providerTenantSettingId}
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
If successful, this method returns a `200 OK` response code and a [providerTenantSetting](../resources/providertenantsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_providertenantsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/providerTenantSettings/{providerTenantSettingId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.providerTenantSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.providerTenantSetting",
    "id": "f801d1a5-d1a5-f801-a5d1-01f8a5d101f8",
    "azureTenantId": "Azure Tenant Id value",
    "enabled": true,
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "provider": "Provider value",
    "vendor": "Vendor value"
  }
}
```

