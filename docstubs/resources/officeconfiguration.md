---
title: "officeConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# officeConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeConfiguration](../api/officeconfiguration-get.md)|[officeConfiguration](../resources/officeconfiguration.md)|Read properties and relationships of the [officeConfiguration](../resources/officeconfiguration.md) object.|
|[Update officeConfiguration](../api/officeconfiguration-update.md)|[officeConfiguration](../resources/officeconfiguration.md)|Update the properties of a [officeConfiguration](../resources/officeconfiguration.md) object.|
|[List clientConfigurations](../api/officeconfiguration-list-clientconfigurations.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md) collection|Get the officeClientConfigurations from the clientConfigurations navigation property.|
|[Add clientConfigurations](../api/officeconfiguration-post-clientconfigurations.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md)|Add clientConfigurations by posting to the clientConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|tenantCheckinStatuses|[officeClientCheckinStatus](../resources/officeclientcheckinstatus.md) collection||
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/officeusercheckinsummary.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|clientConfigurations|[officeClientConfiguration](../resources/officeclientconfiguration.md) collection||

## JSON representation
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

