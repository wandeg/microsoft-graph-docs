---
title: "groupPolicyPresentationDropdownList resource type"
description: "Represents an ADMX dropdownList element and an ADMX enum element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationDropdownList resource type

Represents an ADMX dropdownList element and an ADMX enum element.


Inherits from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationDropdownLists](../api/grouppolicypresentationdropdownlist-list.md)|[groupPolicyPresentationDropdownList](../resources/groupPolicyPresentationDropdownList.md) collection|List properties and relationships of the [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md) objects.|
|[Get groupPolicyPresentationDropdownList](../api/grouppolicypresentationdropdownlist-get.md)|[groupPolicyPresentationDropdownList](../resources/groupPolicyPresentationDropdownList.md)|Read properties and relationships of the [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md) object.|
|[Create groupPolicyPresentationDropdownList](../api/grouppolicypresentationdropdownlist-create.md)|[groupPolicyPresentationDropdownList](../resources/groupPolicyPresentationDropdownList.md)|Create a new [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md) object.|
|[Delete groupPolicyPresentationDropdownList](../api/grouppolicypresentationdropdownlist-delete.md)|None|Deletes a [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md).|
|[Update groupPolicyPresentationDropdownList](../api/grouppolicypresentationdropdownlist-update.md)|[groupPolicyPresentationDropdownList](../resources/groupPolicyPresentationDropdownList.md)|Update the properties of a [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultItem|[groupPolicyPresentationDropdownListItem](../resources/groupPolicyPresentationDropdownListItem.md)|Localized string value identifying the default choice of the list of items.|
|id|String| Inherited from [entity](../resources/entity.md)|
|items|[groupPolicyPresentationDropdownListItem](../resources/groupPolicyPresentationDropdownListItem.md) collection|Represents a set of localized display names and their associated values.|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|required|Boolean|Requirement to enter a value in the parameter box. The default value is false.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownList",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "value": "String"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem"
    }
  ],
  "required": true
}
```

