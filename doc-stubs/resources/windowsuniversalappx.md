---
title: "windowsUniversalAppX resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsUniversalAppX resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [mobileLobApp](../resources/mobilelobapp.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List categories](../api/windowsuniversalappx-list-categories.md)|[mobileAppCategory](../resources/intune-mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Add categories](../api/windowsuniversalappx-post-categories.md)|[mobileAppCategory](../resources/intune-mobileappcategory.md)|Add categories by posting to the categories collection.|
|[Remove categories](../api/windowsuniversalappx-delete-categories.md)|None|Remove a [mobileAppCategory](../resources/intune-mobileappcategory.md) object.|
|[List assignments](../api/windowsuniversalappx-list-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsuniversalappx-post-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsuniversalappx-delete-assignments.md)|None|Delete a [mobileAppAssignment](../resources/intune-mobileappassignment.md) object.|
|[Update assignments](../api/windowsuniversalappx-update-assignments.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/windowsuniversalappx-get-mobileappassignment.md)|[mobileAppAssignment](../resources/intune-mobileappassignment.md)|Read the properties and relationships of a [mobileAppAssignment](../resources/intune-mobileappassignment.md) object.|
|[List contentVersions](../api/windowsuniversalappx-list-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md) collection|Get the mobileAppContents from the contentVersions navigation property.|
|[Create contentVersions](../api/windowsuniversalappx-post-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Create a new contentVersions object.|
|[Delete contentVersions](../api/windowsuniversalappx-delete-contentversions.md)|None|Delete a [mobileAppContent](../resources/intune-mobileappcontent.md) object.|
|[Update contentVersions](../api/windowsuniversalappx-update-contentversions.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Update the properties of a contentVersions object.|
|[Get contentVersions](../api/windowsuniversalappx-get-mobileappcontent.md)|[mobileAppContent](../resources/intune-mobileappcontent.md)|Read the properties and relationships of a [mobileAppContent](../resources/intune-mobileappcontent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableArchitectures|windowsArchitecture|**TODO: Add Description**. Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.|
|applicableDeviceTypes|windowsDeviceType|**TODO: Add Description**. Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.|
|committedContentVersion|String|**TODO: Add Description** Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|description|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|developer|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|displayName|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|fileName|String|**TODO: Add Description** Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|identityName|String|**TODO: Add Description**|
|identityPublisherHash|String|**TODO: Add Description**|
|identityResourceIdentifier|String|**TODO: Add Description**|
|identityVersion|String|**TODO: Add Description**|
|informationUrl|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|isBundle|Boolean|**TODO: Add Description**|
|isFeatured|Boolean|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-mimecontent.md)|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-windowsminimumoperatingsystem.md)|**TODO: Add Description**|
|notes|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|owner|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|privacyInformationUrl|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|publisher|String|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md)|
|publishingState|mobileAppPublishingState|**TODO: Add Description** Inherited from [mobileApp](../resources/intune-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|size|Int64|**TODO: Add Description** Inherited from [mobileLobApp](../resources/mobilelobapp.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-mobileappassignment.md) collection|**TODO: Add Description** Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/intune-mobileappcategory.md) collection|**TODO: Add Description** Inherited from [mobileApp](../resources/mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-mobileappcontent.md) collection|**TODO: Add Description** Inherited from [mobileLobApp](../resources/mobilelobapp.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppX",
  "baseType": "microsoft.graph.mobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": "Integer",
  "applicableArchitectures": "String",
  "applicableDeviceTypes": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "isBundle": "Boolean",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
  },
  "identityVersion": "String"
}
```

