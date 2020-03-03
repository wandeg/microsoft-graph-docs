---
title: "providerTenantSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# providerTenantSetting resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get providerTenantSetting](../api/providertenantsetting-get.md)|[providerTenantSetting](../resources/providerTenantSetting.md)|Read properties and relationships of the [providerTenantSetting](../resources/providertenantsetting.md) object.|
|[Delete providerTenantSetting](../api/providertenantsetting-delete.md)|None|Deletes a [providerTenantSetting](../resources/providertenantsetting.md).|
|[Update providerTenantSetting](../api/providertenantsetting-update.md)|[providerTenantSetting](../resources/providerTenantSetting.md)|Update the properties of a [providerTenantSetting](../resources/providertenantsetting.md) object.|
|[List providerTenantSettings](../api/security-list-providertenantsettings.md)|[providerTenantSetting](../resources/providerTenantSetting.md) collection|Get the providerTenantSettings from the providerTenantSettings navigation property.|
|[Add providerTenantSettings](../api/security-post-providertenantsettings.md)|[providerTenantSetting](../resources/providerTenantSetting.md)|Add providerTenantSettings by posting to the providerTenantSettings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureTenantId|String||
|enabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|provider|String||
|vendor|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.providerTenantSetting",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.providerTenantSetting",
  "id": "String (identifier)",
  "azureTenantId": "String",
  "enabled": true,
  "lastModifiedDateTime": "String (timestamp)",
  "provider": "String",
  "vendor": "String"
}
```

