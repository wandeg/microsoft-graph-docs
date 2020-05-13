---
title: "mobileAppContent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppContent resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List contentVersions](../api/managedmobilelobapp-list-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Create contentVersions](../api/managedmobilelobapp-post-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Create a new contentVersions object.|
|[Delete contentVersions](../api/managedmobilelobapp-delete-contentversions.md)|None|Delete a [mobileAppContent](../resources/intune-mobileappcontent.md) object.|
|[Update contentVersions](../api/managedmobilelobapp-update-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Update the properties of a contentVersions object.|
|[Get contentVersions](../api/managedmobilelobapp-get-mobileappcontent.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Read the properties and relationships of a [mobileAppContent](../resources/intune-mobileappcontent.md) object.|
|[List files](../api/intune-mobileappcontent-list-files.md)|[mobileAppContentFile](../resources/intune-mobileappcontentfile.md) collection|Get the mobileAppContentFiles from the files navigation property.|
|[Create files](../api/intune-mobileappcontent-post-files.md)|[mobileAppContentFile](../resources/intune-mobileappcontentfile.md)|Create a new files object.|
|[Delete files](../api/intune-mobileappcontent-delete-files.md)|None|Delete a [mobileAppContentFile](../resources/intune-mobileappcontentfile.md) object.|
|[Update files](../api/intune-mobileappcontent-update-files.md)|[mobileAppContentFile](../resources/intune-mobileappcontentfile.md)|Update the properties of a files object.|
|[Get files](../api/intune-mobileappcontent-get-mobileappcontentfile.md)|[mobileAppContentFile](../resources/intune-mobileappcontentfile.md)|Read the properties and relationships of a [mobileAppContentFile](../resources/intune-mobileappcontentfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/intune-mobileappcontentfile.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

