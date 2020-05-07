---
title: "sensitivityLabel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sensitivityLabel resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[evaluate](../api/sensitivitylabel-evaluate.md)|[evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md)|**TODO: Add Description**|
|[List sublabels](../api/sensitivitylabel-list-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|Get the sensitivityLabels from the sublabels navigation property.|
|[Create sublabels](../api/sensitivitylabel-post-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Create a new sublabels object.|
|[Delete sublabels](../api/sensitivitylabel-delete-sublabels.md)|None|Delete a [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[Update sublabels](../api/sensitivitylabel-update-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Update the properties of a sublabels object.|
|[Get sensitivityLabel](../api/sensitivitylabel-get.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Read the properties and relationships of a [sensitivityLabel](../resources/sensitivitylabel.md) object.|
|[List sublabels](../api/sensitivitylabel-list-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|Get the sensitivityLabels from the sublabels navigation property.|
|[Create sublabels](../api/sensitivitylabel-post-sublabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Create a new sublabels object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableTo|sensitivityLabelTarget|**TODO: Add Description**. Possible values are: `email`, `site`, `unifiedGroup`, `unknownFutureValue`.|
|applicationMode|applicationMode|**TODO: Add Description**. Possible values are: `manual`, `automatic`, `recommended`.|
|assignedPolicies|[labelPolicy](../resources/labelpolicy.md) collection|**TODO: Add Description**|
|autoLabeling|[autoLabeling](../resources/autolabeling.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|**TODO: Add Description**|
|isEndpointProtectionEnabled|Boolean|**TODO: Add Description**|
|labelActions|[labelActionBase](../resources/labelactionbase.md) collection|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|toolTip|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sublabels|[sensitivityLabel](../resources/sensitivitylabel.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "isEndpointProtectionEnabled": "Boolean",
  "isDefault": "Boolean",
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
  "priority": "Integer",
  "autoLabeling": {
    "@odata.type": "microsoft.graph.autoLabeling"
  },
  "applicableTo": "String"
}
```

