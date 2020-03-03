---
title: "microsoftStoreForBusinessApp resource type"
description: "Microsoft Store for Business Apps. This class does not support Create, Delete, or Update."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# microsoftStoreForBusinessApp resource type


Namespace: microsoft.graph

Microsoft Store for Business Apps. This class does not support Create, Delete, or Update.


Inherits from [mobileApp](../resources/mobileapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List microsoftStoreForBusinessApps](../api/microsoftstoreforbusinessapp-list.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) collection|List properties and relationships of the [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) objects.|
|[Get microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-get.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md)|Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) object.|
|[Create microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-create.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md)|Create a new [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) object.|
|[Delete microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-delete.md)|None|Deletes a [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md).|
|[Update microsoftStoreForBusinessApp](../api/microsoftstoreforbusinessapp-update.md)|[microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md)|Update the properties of a [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) object.|
|[assign](../api/microsoftstoreforbusinessapp-assign.md)|None||
|[List categories](../api/microsoftstoreforbusinessapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/microsoftstoreforbusinessapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/microsoftstoreforbusinessapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/microsoftstoreforbusinessapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Add assignments by posting to the assignments collection.|

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
|licenseType|Enumeration|The app license type. Possible values are: `offline`, `online`.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|packageIdentityName|String|The app package identifier|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|productKey|String|The app product key|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|totalLicenseCount|Int32|The total number of Microsoft Store for Business licenses.|
|usedLicenseCount|Int32|The number of Microsoft Store for Business licenses in use.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp",
  "baseType": "microsoft.graph.mobileApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "publishingState": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String"
}
```

