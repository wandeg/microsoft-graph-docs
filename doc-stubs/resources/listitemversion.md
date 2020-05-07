---
title: "listItemVersion resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# listItemVersion resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItemVersion](../resources/baseitemversion.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[restoreVersion](../api/listitemversion-restoreversion.md)|None|**TODO: Add Description**|
|[List fields](../api/listitemversion-list-fields.md)|[fieldValueSet](../resources/fieldvalueset.md) collection|Get the fieldValueSets from the fields navigation property.|
|[Create fields](../api/listitemversion-post-fields.md)|[fieldValueSet](../resources/fieldvalueset.md)|Create a new fields object.|
|[Delete fields](../api/listitemversion-delete-fields.md)|None|Delete a [fieldValueSet](../resources/fieldvalueset.md) object.|
|[Update fields](../api/listitemversion-update-fields.md)|[fieldValueSet](../resources/fieldvalueset.md)|Update the properties of a fields object.|
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldvalueset.md)|Read the properties and relationships of a [fieldValueSet](../resources/fieldvalueset.md) object.|
|[List versions](../api/listitem-list-versions.md)|[listItemVersion](../resources/listitemversion.md) collection|Get the listItemVersions from the versions navigation property.|
|[Create versions](../api/listitem-post-versions.md)|[listItemVersion](../resources/listitemversion.md)|Create a new versions object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fields|[fieldValueSet](../resources/fieldvalueset.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.listItemVersion",
  "baseType": "microsoft.graph.baseItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.listItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  }
}
```

