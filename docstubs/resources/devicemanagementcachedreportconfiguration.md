---
title: "deviceManagementCachedReportConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementCachedReportConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[Update deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Update the properties of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[List cachedReportConfigurations](../api/devicemanagementreports-list-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection|Get the deviceManagementCachedReportConfigurations from the cachedReportConfigurations navigation property.|
|[Add cachedReportConfigurations](../api/devicemanagementreports-post-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Add cachedReportConfigurations by posting to the cachedReportConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset||
|filter|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastRefreshDateTime|DateTimeOffset||
|orderBy|String collection||
|reportName|String||
|select|String collection||
|status|Enumeration| Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```

