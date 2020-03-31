---
title: "providerTenantSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# providerTenantSetting resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get providerTenantSetting](../api/providertenantsetting-get.md)|[providerTenantSetting](../resources/providertenantsetting.md)|Read properties and relationships of the [providerTenantSetting](../resources/providertenantsetting.md) object.|
|[Update providerTenantSetting](../api/providertenantsetting-update.md)|[providerTenantSetting](../resources/providertenantsetting.md)|Update the properties of a [providerTenantSetting](../resources/providertenantsetting.md) object.|

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

## JSON representation
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

