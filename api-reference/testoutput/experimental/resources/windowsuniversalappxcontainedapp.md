---
title: "windowsUniversalAppXContainedApp resource type"
description: "A class that represents a contained app of a WindowsUniversalAppX app."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsUniversalAppXContainedApp resource type


Namespace: microsoft.graph

A class that represents a contained app of a WindowsUniversalAppX app.


Inherits from [mobileContainedApp](../resources/mobilecontainedapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsUniversalAppXContainedApps](../api/windowsuniversalappxcontainedapp-list.md)|[windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) collection|List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) objects.|
|[Get windowsUniversalAppXContainedApp](../api/windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md)|Read properties and relationships of the [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) object.|
|[Create windowsUniversalAppXContainedApp](../api/windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md)|Create a new [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) object.|
|[Delete windowsUniversalAppXContainedApp](../api/windowsuniversalappxcontainedapp-delete.md)|None|Deletes a [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md).|
|[Update windowsUniversalAppXContainedApp](../api/windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md)|Update the properties of a [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appUserModelId|String|The app user model ID of the contained app of a WindowsUniversalAppX app.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppXContainedApp",
  "baseType": "microsoft.graph.mobileContainedApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```

