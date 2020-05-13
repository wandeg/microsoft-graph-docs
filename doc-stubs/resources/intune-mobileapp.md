---
title: "mobileApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List mobileApps](../api/intune-deviceappmanagement-list-mobileapps.md)|[mobileApp](../resources/intune-mobileapp.md) collection|Get the mobileApps from the mobileApps navigation property.|
|[Create mobileApps](../api/intune-deviceappmanagement-post-mobileapps.md)|[mobileApp](../resources/intune-mobileapp.md)|Create a new mobileApps object.|
|[Delete mobileApps](../api/intune-deviceappmanagement-delete-mobileapps.md)|None|Delete a [mobileApp](../resources/intune-mobileapp.md) object.|
|[Update mobileApps](../api/intune-deviceappmanagement-update-mobileapps.md)|[mobileApp](../resources/intune-mobileapp.md)|Update the properties of a mobileApps object.|
|[Get mobileApps](../api/intune-deviceappmanagement-get-mobileapp.md)|[mobileApp](../resources/intune-mobileapp.md)|Read the properties and relationships of a [mobileApp](../resources/intune-mobileapp.md) object.|
|[assign](../api/intune-mobileapp-assign.md)|None|**TODO: Add Description**|
|[List categories](../api/intune-mobileapp-list-categories.md)|[mobileAppCategory](../resources/intune-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Add categories](../api/intune-mobileapp-post-categories.md)|[mobileAppCategory](../resources/intune-mobileappcategory.md)|Add categories by posting to the categories collection.|
|[Remove categories](../api/intune-mobileapp-delete-categories.md)|None|Remove a [mobileAppCategory](../resources/intune-mobileappcategory.md) object.|
|[List assignments](../api/intune-mobileapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Create assignments](../api/intune-mobileapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/intune-mobileapp-delete-assignments.md)|None|Delete a [mobileAppAssignment](../resources/intune-mobileappassignment.md) object.|
|[Update assignments](../api/intune-mobileapp-update-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/intune-mobileapp-get-mobileappassignment.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Read the properties and relationships of a [mobileAppAssignment](../resources/intune-mobileappassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|developer|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|**TODO: Add Description**|
|isFeatured|Boolean|**TODO: Add Description**|
|largeIcon|[mimeContent](../resources/intune-mimecontent.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|notes|String|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|privacyInformationUrl|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|publishingState|mobileAppPublishingState|**TODO: Add Description**. Possible values are: `notPublished`, `processing`, `published`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-mobileappassignment.md) collection|**TODO: Add Description**|
|categories|[mobileAppCategory](../resources/intune-mobileappcategory.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": "Boolean",
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```

