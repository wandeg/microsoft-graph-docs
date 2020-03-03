---
title: "educationOneNoteResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationOneNoteResource resource type




Inherits from [educationResource](../resources/educationResource.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [educationResource](../resources/educationResource.md)|
|createdDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationResource.md)|
|displayName|String| Inherited from [educationResource](../resources/educationResource.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationResource](../resources/educationResource.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationResource.md)|
|pageUrl|String||
|sectionName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationOneNoteResource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
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
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sectionName": "String",
  "pageUrl": "String"
}
```

