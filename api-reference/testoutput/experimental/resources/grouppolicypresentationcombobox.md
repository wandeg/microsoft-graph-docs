---
title: "groupPolicyPresentationComboBox resource type"
description: "Represents an ADMX comboBox element and an ADMX text element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationComboBox resource type


Namespace: microsoft.graph

Represents an ADMX comboBox element and an ADMX text element.


Inherits from [groupPolicyPresentation](../resources/grouppolicypresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationComboBoxes](../api/grouppolicypresentationcombobox-list.md)|[groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md) collection|List properties and relationships of the [groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md) objects.|
|[Get groupPolicyPresentationComboBox](../api/grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md)|Read properties and relationships of the [groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md) object.|
|[Create groupPolicyPresentationComboBox](../api/grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md)|Create a new [groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md) object.|
|[Delete groupPolicyPresentationComboBox](../api/grouppolicypresentationcombobox-delete.md)|None|Deletes a [groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md).|
|[Update groupPolicyPresentationComboBox](../api/grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md)|Update the properties of a [groupPolicyPresentationComboBox](../resources/grouppolicypresentationcombobox.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultValue|String|Localized default string displayed in the combo box. The default value is empty.|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|maxLength|Int64|An unsigned integer that specifies the maximum number of text characters for the parameter. The default value is 1023.|
|required|Boolean|Specifies whether a value must be specified for the parameter. The default value is false.|
|suggestions|String collection|Localized strings listed in the drop-down list of the combo box. The default value is empty.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationComboBox",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "suggestions": [
    "String"
  ],
  "required": true,
  "maxLength": 1024
}
```

