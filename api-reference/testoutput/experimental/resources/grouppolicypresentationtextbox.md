---
title: "groupPolicyPresentationTextBox resource type"
description: "Represents an ADMX textBox element and an ADMX text element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationTextBox resource type

Represents an ADMX textBox element and an ADMX text element.


Inherits from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationTextBoxes](../api/grouppolicypresentationtextbox-list.md)|[groupPolicyPresentationTextBox](../resources/groupPolicyPresentationTextBox.md) collection|List properties and relationships of the [groupPolicyPresentationTextBox](../resources/grouppolicypresentationtextbox.md) objects.|
|[Get groupPolicyPresentationTextBox](../api/grouppolicypresentationtextbox-get.md)|[groupPolicyPresentationTextBox](../resources/groupPolicyPresentationTextBox.md)|Read properties and relationships of the [groupPolicyPresentationTextBox](../resources/grouppolicypresentationtextbox.md) object.|
|[Create groupPolicyPresentationTextBox](../api/grouppolicypresentationtextbox-create.md)|[groupPolicyPresentationTextBox](../resources/groupPolicyPresentationTextBox.md)|Create a new [groupPolicyPresentationTextBox](../resources/grouppolicypresentationtextbox.md) object.|
|[Delete groupPolicyPresentationTextBox](../api/grouppolicypresentationtextbox-delete.md)|None|Deletes a [groupPolicyPresentationTextBox](../resources/grouppolicypresentationtextbox.md).|
|[Update groupPolicyPresentationTextBox](../api/grouppolicypresentationtextbox-update.md)|[groupPolicyPresentationTextBox](../resources/groupPolicyPresentationTextBox.md)|Update the properties of a [groupPolicyPresentationTextBox](../resources/grouppolicypresentationtextbox.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultValue|String|Localized default string displayed in the text box. The default value is empty.|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|maxLength|Int64|An unsigned integer that specifies the maximum number of text characters. Default value is 1023.|
|required|Boolean|Requirement to enter a value in the text box. Default value is false.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationTextBox",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "required": true,
  "maxLength": 1024
}
```

