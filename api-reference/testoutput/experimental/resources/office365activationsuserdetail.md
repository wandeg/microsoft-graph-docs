---
title: "office365ActivationsUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# office365ActivationsUserDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365ActivationsUserDetails](../api/office365activationsuserdetail-list.md)|[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) collection|List properties and relationships of the [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) objects.|
|[Get office365ActivationsUserDetail](../api/office365activationsuserdetail-get.md)|[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)|Read properties and relationships of the [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object.|
|[Create office365ActivationsUserDetail](../api/office365activationsuserdetail-create.md)|[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)|Create a new [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object.|
|[Delete office365ActivationsUserDetail](../api/office365activationsuserdetail-delete.md)|None|Deletes a [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md).|
|[Update office365ActivationsUserDetail](../api/office365activationsuserdetail-update.md)|[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)|Update the properties of a [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userActivationCounts|[userActivationCounts](../resources/useractivationcounts.md) collection||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365ActivationsUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "userActivationCounts": [
    {
      "@odata.type": "microsoft.graph.userActivationCounts"
    }
  ]
}
```

