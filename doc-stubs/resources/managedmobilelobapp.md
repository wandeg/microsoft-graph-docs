---
title: "managedMobileLobApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedMobileLobApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managedApp](../resources/managedapp.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List categories](../api/managedmobilelobapp-list-categories.md)|[mobileAppCategory](../resources/intune-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Add categories](../api/managedmobilelobapp-post-categories.md)|[mobileAppCategory](../resources/intune-mobileappcategory.md)|Add categories by posting to the categories collection.|
|[Remove categories](../api/managedmobilelobapp-delete-categories.md)|None|Remove a [mobileAppCategory](../resources/intune-mobileappcategory.md) object.|
|[List assignments](../api/managedmobilelobapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Create assignments](../api/managedmobilelobapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/managedmobilelobapp-delete-assignments.md)|None|Delete a [mobileAppAssignment](../resources/intune-mobileappassignment.md) object.|
|[Update assignments](../api/managedmobilelobapp-update-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/managedmobilelobapp-get-mobileappassignment.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Read the properties and relationships of a [mobileAppAssignment](../resources/intune-mobileappassignment.md) object.|
|[List contentVersions](../api/managedmobilelobapp-list-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Create contentVersions](../api/managedmobilelobapp-post-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Create a new contentVersions object.|
|[Delete contentVersions](../api/managedmobilelobapp-delete-contentversions.md)|None|Delete a [mobileAppContent](../resources/intune-mobileappcontent.md) object.|
|[Update contentVersions](../api/managedmobilelobapp-update-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Update the properties of a contentVersions object.|
|[Get contentVersions](../api/managedmobilelobapp-get-mobileappcontent.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Read the properties and relationships of a [mobileAppContent](../resources/intune-mobileappcontent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAvailability|managedAppAvailability|**TODO: Add Description** Inherited from [managedApp](../resources/managedapp.md). Possible values are: `global`, `lineOfBusiness`.|
|committedContentVersion|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|description|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|developer|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|displayName|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|fileName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|isFeatured|Boolean|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-mimecontent.md)|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|notes|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|owner|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|privacyInformationUrl|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|publisher|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|publishingState|mobileAppPublishingState|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|size|Int64|**TODO: Add Description**|
|version|String|**TODO: Add Description** Inherited from [managedApp](../resources/managedapp.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-mobileappassignment.md) collection|**TODO: Add Description** Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/intune-mobileappcategory.md) collection|**TODO: Add Description** Inherited from [mobileApp](../resources/mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-mobileappcontent.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileLobApp",
  "baseType": "microsoft.graph.managedApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileLobApp",
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
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": "Integer"
}
```

