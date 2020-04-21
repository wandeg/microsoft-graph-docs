---
title: "listItemVersion resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# listItemVersion resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItemVersion](../resources/baseitemversion.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get listItemVersion](../api/listitemversion-get.md)|[listItemVersion](../resources/listitemversion.md)|Read properties and relationships of a [listItemVersion](../resources/listitemversion.md) object.|
|[Update listItemVersion](../api/listitemversion-update.md)|[listItemVersion](../resources/listitemversion.md)|Update the properties of a [listItemVersion](../resources/listitemversion.md) object.|
|[restoreVersion](../api/listitemversion-restoreversion.md)|None|**TODO: Add Description**|
|[List fields](../api/listitemversion-list-fields.md)|[fieldValueSet](../resources/fieldvalueset.md) collection|Get the fieldValueSets from the fields navigation property.|
|[Create fields](../api/listitemversion-post-fields.md)|[fieldValueSet](../resources/fieldvalueset.md)|Create a new fields object.|
|[Delete fields](../api/listitemversion-delete-fields.md)|None|Delete a fields object.|
|[Update fields](../api/listitemversion-update-fields.md)|[fieldValueSet](../resources/fieldvalueset.md)|Update the properties of a fields object.|
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldvalueset.md)|Read properties and relationships of a [fieldValueSet](../resources/fieldvalueset.md) object.|
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
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "String",
    "versionId": "String"
  }
}
```

