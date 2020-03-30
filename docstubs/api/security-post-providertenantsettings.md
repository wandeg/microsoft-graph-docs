---
title: "Add providerTenantSettings"
description: "Add providerTenantSettings by posting to the providerTenantSettings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add providerTenantSettings

Namespace: microsoft.graph

Add providerTenantSettings by posting to the providerTenantSettings collection.

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
POST /Security/providerTenantSettings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [providerTenantSetting](../resources/providertenantsetting.md) object.

The following table shows the properties that are required when you create the [providerTenantSetting](../resources/providertenantsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|azureTenantId|String||
|enabled|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|provider|String||
|vendor|String||



## Response
If successful, this method returns a `201 Created` response code and a [providerTenantSetting](../resources/providertenantsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_providertenantsetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/providerTenantSettings
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.providertenantsetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 303

{
  "@odata.type": "#microsoft.graph.providerTenantSetting",
  "id": "9a3775c3-75c3-9a37-c375-379ac375379a",
  "azureTenantId": "Azure Tenant Id value",
  "enabled": true,
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
  "provider": "Provider value",
  "vendor": "Vendor value"
}
```

