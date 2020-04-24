---
title: "Create providerTenantSettings"
description: "Create a new providerTenantSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create providerTenantSettings

Namespace: microsoft.graph

Create a new providerTenantSettings object.

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
POST /Security/providerTenantSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [providerTenantSetting](../resources/providertenantsetting.md) object.

The following table shows the properties that are required when you create the [providerTenantSetting](../resources/providertenantsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|azureTenantId|String|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|provider|String|**TODO: Add Description**|
|vendor|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [providerTenantSetting](../resources/providertenantsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_providertenantsetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/providerTenantSettings
Content-Type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.providerTenantSetting",
  "azureTenantId": "Azure Tenant Id value",
  "enabled": true,
  "provider": "Provider value",
  "vendor": "Vendor value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.providertenantsetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.providerTenantSetting",
  "id": "f801d1a5-d1a5-f801-a5d1-01f8a5d101f8",
  "azureTenantId": "Azure Tenant Id value",
  "enabled": true,
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "provider": "Provider value",
  "vendor": "Vendor value"
}
```

