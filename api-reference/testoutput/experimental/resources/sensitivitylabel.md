---
title: "sensitivityLabel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sensitivityLabel resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sensitivityLabels](../api/sensitivitylabel-list.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|List properties and relationships of the [sensitivityLabel](../resources/sensitivitylabel.md) objects.|
|[Get sensitivityLabel](../api/sensitivitylabel-get.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Read properties and relationships of the [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[Create sensitivityLabel](../api/sensitivitylabel-create.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Create a new [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[Delete sensitivityLabel](../api/sensitivitylabel-delete.md)|None|Deletes a [sensitivityLabel](../resources/sensitivitylabel.md).|
|[Update sensitivityLabel](../api/sensitivitylabel-update.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Update the properties of a [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[evaluate](../api/sensitivitylabel-evaluate.md)|[evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md)||
|[List sublabels](../api/sensitivitylabel-list-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|Get the sensitivityLabels from the sublabels navigation property.|
|[Add sublabels](../api/sensitivitylabel-post-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Add sublabels by posting to the sublabels collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationMode|Enumeration|. Possible values are: `manual`, `automatic`, `recommended`.|
|assignedPolicies|[labelPolicy](../resources/labelpolicy.md) collection||
|autoLabeling|[autoLabeling](../resources/autolabeling.md)||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|isEndpointProtectionEnabled|Boolean||
|labelActions|[labelActionBase](../resources/labelactionbase.md) collection||
|name|String||
|priority|Int32||
|toolTip|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sublabels|[sensitivityLabel](../resources/sensitivitylabel.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sensitivityLabel",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitivityLabel",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "toolTip": "String",
  "isEndpointProtectionEnabled": true,
  "isDefault": true,
  "applicationMode": "String",
  "labelActions": [
    {
      "@odata.type": "microsoft.graph.encryptWithUserDefinedRights"
    }
  ],
  "assignedPolicies": [
    {
      "@odata.type": "microsoft.graph.labelPolicy"
    }
  ],
  "priority": 1024,
  "autoLabeling": {
    "@odata.type": "microsoft.graph.autoLabeling"
  }
}
```

