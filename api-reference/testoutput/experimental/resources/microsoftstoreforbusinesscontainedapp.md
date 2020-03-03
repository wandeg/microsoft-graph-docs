---
title: "microsoftStoreForBusinessContainedApp resource type"
description: "A class that represents a contained app of a MicrosoftStoreForBusinessApp."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# microsoftStoreForBusinessContainedApp resource type


Namespace: microsoft.graph

A class that represents a contained app of a MicrosoftStoreForBusinessApp.


Inherits from [mobileContainedApp](../resources/mobilecontainedapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List microsoftStoreForBusinessContainedApps](../api/microsoftstoreforbusinesscontainedapp-list.md)|[microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) collection|List properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) objects.|
|[Get microsoftStoreForBusinessContainedApp](../api/microsoftstoreforbusinesscontainedapp-get.md)|[microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md)|Read properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) object.|
|[Create microsoftStoreForBusinessContainedApp](../api/microsoftstoreforbusinesscontainedapp-create.md)|[microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md)|Create a new [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) object.|
|[Delete microsoftStoreForBusinessContainedApp](../api/microsoftstoreforbusinesscontainedapp-delete.md)|None|Deletes a [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md).|
|[Update microsoftStoreForBusinessContainedApp](../api/microsoftstoreforbusinesscontainedapp-update.md)|[microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md)|Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appUserModelId|String|The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessContainedApp",
  "baseType": "microsoft.graph.mobileContainedApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```

