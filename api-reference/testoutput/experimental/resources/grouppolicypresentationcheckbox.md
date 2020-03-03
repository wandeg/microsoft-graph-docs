---
title: "groupPolicyPresentationCheckBox resource type"
description: "Represents an ADMX checkBox element and an ADMX boolean element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationCheckBox resource type


Namespace: microsoft.graph

Represents an ADMX checkBox element and an ADMX boolean element.


Inherits from [groupPolicyPresentation](../resources/grouppolicypresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationCheckBoxes](../api/grouppolicypresentationcheckbox-list.md)|[groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) collection|List properties and relationships of the [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) objects.|
|[Get groupPolicyPresentationCheckBox](../api/grouppolicypresentationcheckbox-get.md)|[groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md)|Read properties and relationships of the [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) object.|
|[Create groupPolicyPresentationCheckBox](../api/grouppolicypresentationcheckbox-create.md)|[groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md)|Create a new [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) object.|
|[Delete groupPolicyPresentationCheckBox](../api/grouppolicypresentationcheckbox-delete.md)|None|Deletes a [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md).|
|[Update groupPolicyPresentationCheckBox](../api/grouppolicypresentationcheckbox-update.md)|[groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md)|Update the properties of a [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultChecked|Boolean|Default value for the check box. The default value is false.|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/grouppolicypresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationCheckBox",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultChecked": true
}
```

