---
title: "mailboxUsageStorage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mailboxUsageStorage resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailboxUsageStorages](../api/mailboxusagestorage-list.md)|[mailboxUsageStorage](../resources/mailboxUsageStorage.md) collection|List properties and relationships of the [mailboxUsageStorage](../resources/mailboxusagestorage.md) objects.|
|[Get mailboxUsageStorage](../api/mailboxusagestorage-get.md)|[mailboxUsageStorage](../resources/mailboxUsageStorage.md)|Read properties and relationships of the [mailboxUsageStorage](../resources/mailboxusagestorage.md) object.|
|[Create mailboxUsageStorage](../api/mailboxusagestorage-create.md)|[mailboxUsageStorage](../resources/mailboxUsageStorage.md)|Create a new [mailboxUsageStorage](../resources/mailboxusagestorage.md) object.|
|[Delete mailboxUsageStorage](../api/mailboxusagestorage-delete.md)|None|Deletes a [mailboxUsageStorage](../resources/mailboxusagestorage.md).|
|[Update mailboxUsageStorage](../api/mailboxusagestorage-update.md)|[mailboxUsageStorage](../resources/mailboxUsageStorage.md)|Update the properties of a [mailboxUsageStorage](../resources/mailboxusagestorage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|storageUsedInBytes|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailboxUsageStorage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailboxUsageStorage",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "storageUsedInBytes": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

