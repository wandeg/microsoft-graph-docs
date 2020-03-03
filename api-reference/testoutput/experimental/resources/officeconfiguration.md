---
title: "officeConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# officeConfiguration resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeConfiguration](../api/officeconfiguration-get.md)|[officeConfiguration](../resources/officeConfiguration.md)|Read properties and relationships of the [officeConfiguration](../resources/officeconfiguration.md) object.|
|[Update officeConfiguration](../api/officeconfiguration-update.md)|[officeConfiguration](../resources/officeConfiguration.md)|Update the properties of a [officeConfiguration](../resources/officeconfiguration.md) object.|
|[List clientConfigurations](../api/officeconfiguration-list-clientconfigurations.md)|[officeClientConfiguration](../resources/officeClientConfiguration.md) collection|Get the officeClientConfigurations from the clientConfigurations navigation property.|
|[Add clientConfigurations](../api/officeconfiguration-post-clientconfigurations.md)|[officeClientConfiguration](../resources/officeClientConfiguration.md)|Add clientConfigurations by posting to the clientConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|tenantCheckinStatuses|[officeClientCheckinStatus](../resources/officeClientCheckinStatus.md) collection||
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/officeUserCheckinSummary.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|clientConfigurations|[officeClientConfiguration](../resources/officeClientConfiguration.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary"
  }
}
```

