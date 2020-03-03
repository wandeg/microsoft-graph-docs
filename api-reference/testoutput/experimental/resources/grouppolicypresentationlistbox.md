---
title: "groupPolicyPresentationListBox resource type"
description: "Represents an ADMX listBox element and an ADMX list element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationListBox resource type

Represents an ADMX listBox element and an ADMX list element.


Inherits from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationListBoxes](../api/grouppolicypresentationlistbox-list.md)|[groupPolicyPresentationListBox](../resources/groupPolicyPresentationListBox.md) collection|List properties and relationships of the [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md) objects.|
|[Get groupPolicyPresentationListBox](../api/grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/groupPolicyPresentationListBox.md)|Read properties and relationships of the [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md) object.|
|[Create groupPolicyPresentationListBox](../api/grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/groupPolicyPresentationListBox.md)|Create a new [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md) object.|
|[Delete groupPolicyPresentationListBox](../api/grouppolicypresentationlistbox-delete.md)|None|Deletes a [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md).|
|[Update groupPolicyPresentationListBox](../api/grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/groupPolicyPresentationListBox.md)|Update the properties of a [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|explicitValue|Boolean|If this option is specified true the user must specify the registry subkey value and the registry subkey name. The list box shows two columns, one for the name and one for the data. The default value is false.|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|valuePrefix|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "explicitValue": true,
  "valuePrefix": "String"
}
```

