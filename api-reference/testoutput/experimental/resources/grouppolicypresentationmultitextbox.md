---
title: "groupPolicyPresentationMultiTextBox resource type"
description: "Represents an ADMX multiTextBox element and an ADMX multiText element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationMultiTextBox resource type


Namespace: microsoft.graph

Represents an ADMX multiTextBox element and an ADMX multiText element.


Inherits from [groupPolicyPresentation](../resources/grouppolicypresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationMultiTextBoxes](../api/grouppolicypresentationmultitextbox-list.md)|[groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) collection|List properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) objects.|
|[Get groupPolicyPresentationMultiTextBox](../api/grouppolicypresentationmultitextbox-get.md)|[groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md)|Read properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) object.|
|[Create groupPolicyPresentationMultiTextBox](../api/grouppolicypresentationmultitextbox-create.md)|[groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md)|Create a new [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) object.|
|[Delete groupPolicyPresentationMultiTextBox](../api/grouppolicypresentationmultitextbox-delete.md)|None|Deletes a [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md).|
|[Update groupPolicyPresentationMultiTextBox](../api/grouppolicypresentationmultitextbox-update.md)|[groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md)|Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/grouppolicypresentationmultitextbox.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|maxLength|Int64|An unsigned integer that specifies the maximum number of text characters. Default value is 1023.|
|maxStrings|Int64|An unsigned integer that specifies the maximum number of strings. Default value is 0.|
|required|Boolean|Requirement to enter a value in the text box. Default value is false.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```

