---
title: "mobileAppContent resource type"
description: "Contains content properties for a specific app version. Each mobileAppContent can have multiple mobileAppContentFile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppContent resource type


Namespace: microsoft.graph

Contains content properties for a specific app version. Each mobileAppContent can have multiple mobileAppContentFile.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppContents](../api/intune-apps-mobileappcontent-list.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection|List properties and relationships of the [mobileAppContent](../resources/mobileappcontent.md) objects.|
|[Get mobileAppContent](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.|
|[Create mobileAppContent](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.|
|[Delete mobileAppContent](../api/intune-apps-mobileappcontent-delete.md)|None|Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Update mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.|
|[List files](../api/intune-apps-mobileappcontent-list-files.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection|Get the mobileAppContentFiles from the files navigation property.|
|[Add files](../api/intune-apps-mobileappcontent-post-files.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Add files by posting to the files collection.|
|[List containedApps](../api/intune-apps-mobileappcontent-list-containedapps.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection|Get the mobileContainedApps from the containedApps navigation property.|
|[Add containedApps](../api/intune-apps-mobileappcontent-post-containedapps.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Add containedApps by posting to the containedApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection|The collection of contained apps in a MobileLobApp acting as a package.|
|files|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection|The list of files for this app content version.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```

