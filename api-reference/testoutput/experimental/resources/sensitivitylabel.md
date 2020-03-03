---
title: "sensitivityLabel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sensitivityLabel resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sensitivityLabel](../api/sensitivitylabel-get.md)|[sensitivityLabel](../resources/sensitivityLabel.md)|Read properties and relationships of the [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[Delete sensitivityLabel](../api/sensitivitylabel-delete.md)|None|Deletes a [sensitivityLabel](../resources/sensitivitylabel.md).|
|[Update sensitivityLabel](../api/sensitivitylabel-update.md)|[sensitivityLabel](../resources/sensitivityLabel.md)|Update the properties of a [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[evaluate](../api/sensitivitylabel-evaluate.md)|[evaluateLabelJobResponse](../resources/evaluateLabelJobResponse.md)||
|[List sublabels](../api/sensitivitylabel-list-sublabels.md)|[sensitivityLabel](../resources/sensitivityLabel.md) collection|Get the sensitivityLabels from the sublabels navigation property.|
|[Add sublabels](../api/sensitivitylabel-post-sublabels.md)|[sensitivityLabel](../resources/sensitivityLabel.md)|Add sublabels by posting to the sublabels collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationMode|Enumeration|. Possible values are: `manual`, `automatic`, `recommended`.|
|assignedPolicies|[labelPolicy](../resources/labelPolicy.md) collection||
|autoLabeling|[autoLabeling](../resources/autoLabeling.md)||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|isEndpointProtectionEnabled|Boolean||
|labelActions|[labelActionBase](../resources/labelActionBase.md) collection||
|name|String||
|priority|Int32||
|toolTip|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sublabels|[sensitivityLabel](../resources/sensitivityLabel.md) collection||

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

