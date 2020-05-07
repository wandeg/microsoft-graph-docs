---
title: "officeConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# officeConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get officeConfiguration](../api/officeconfiguration-get.md)|[officeConfiguration](../resources/officeconfiguration.md)|Read the properties and relationships of an [officeConfiguration](../resources/officeconfiguration.md) object.|
|[Update officeConfiguration](../api/officeconfiguration-update.md)|[officeConfiguration](../resources/officeconfiguration.md)|Update the properties of an [officeConfiguration](../resources/officeconfiguration.md) object.|
|[List clientConfigurations](../api/officeconfiguration-list-clientconfigurations.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md) collection|Get the officeClientConfigurations from the clientConfigurations navigation property.|
|[Create clientConfigurations](../api/officeconfiguration-post-clientconfigurations.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md)|Create a new clientConfigurations object.|
|[Delete clientConfigurations](../api/officeconfiguration-delete-clientconfigurations.md)|None|Delete a [officeClientConfiguration](../resources/officeclientconfiguration.md) object.|
|[Update clientConfigurations](../api/officeconfiguration-update-clientconfigurations.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md)|Update the properties of a clientConfigurations object.|
|[Get officeClientConfiguration](../api/officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/officeclientconfiguration.md)|Read the properties and relationships of an [officeClientConfiguration](../resources/officeclientconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|tenantCheckinStatuses|[officeClientCheckinStatus](../resources/officeclientcheckinstatus.md) collection|**TODO: Add Description**|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/officeusercheckinsummary.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|clientConfigurations|[officeClientConfiguration](../resources/officeclientconfiguration.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

