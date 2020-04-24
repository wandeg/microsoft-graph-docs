---
title: "providerTenantSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# providerTenantSetting resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get providerTenantSetting](../api/providertenantsetting-get.md)|[providerTenantSetting](../resources/providertenantsetting.md)|Read the properties and relationships of a [providerTenantSetting](../resources/providertenantsetting.md) object.|
|[Update providerTenantSetting](../api/providertenantsetting-update.md)|[providerTenantSetting](../resources/providertenantsetting.md)|Update the properties of a [providerTenantSetting](../resources/providertenantsetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureTenantId|String|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|provider|String|**TODO: Add Description**|
|vendor|String|**TODO: Add Description**|

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

