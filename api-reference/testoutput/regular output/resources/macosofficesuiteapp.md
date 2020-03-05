---
title: "macOSOfficeSuiteApp resource type"
description: "Contains properties and inherited properties for the MacOS Office Suite App."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# macOSOfficeSuiteApp resource type


Namespace: microsoft.graph

Contains properties and inherited properties for the MacOS Office Suite App.


Inherits from [mobileApp](../resources/mobileapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List macOSOfficeSuiteApps](../api/macosofficesuiteapp-list.md)|[macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md) collection|List properties and relationships of the [macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md) objects.|
|[Get macOSOfficeSuiteApp](../api/macosofficesuiteapp-get.md)|[macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md)|Read properties and relationships of the [macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md) object.|
|[Create macOSOfficeSuiteApp](../api/macosofficesuiteapp-create.md)|[macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md)|Create a new [macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md) object.|
|[Delete macOSOfficeSuiteApp](../api/macosofficesuiteapp-delete.md)|None|Deletes a [macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md).|
|[Update macOSOfficeSuiteApp](../api/macosofficesuiteapp-update.md)|[macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md)|Update the properties of a [macOSOfficeSuiteApp](../resources/macosofficesuiteapp.md) object.|
|[assign](../api/macosofficesuiteapp-assign.md)|None||
|[List categories](../api/macosofficesuiteapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/macosofficesuiteapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/macosofficesuiteapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/macosofficesuiteapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md)|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSOfficeSuiteApp",
  "baseType": "microsoft.graph.mobileApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```

