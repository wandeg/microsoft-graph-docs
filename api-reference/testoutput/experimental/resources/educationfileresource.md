---
title: "educationFileResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationFileResource resource type


Namespace: microsoft.graph




Inherits from [educationResource](../resources/educationresource.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [educationResource](../resources/educationresource.md)|
|createdDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationresource.md)|
|displayName|String| Inherited from [educationResource](../resources/educationresource.md)|
|fileUrl|String||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [educationResource](../resources/educationresource.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationresource.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationFileResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationFileResource",
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
  "fileUrl": "String"
}
```

