---
title: "educationFormResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationFormResource resource type




Inherits from [educationResource](../resources/educationResource.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [educationResource](../resources/educationResource.md)|
|createdDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationResource.md)|
|displayName|String| Inherited from [educationResource](../resources/educationResource.md)|
|editUrl|String||
|formId|String||
|isGroupForm|Boolean||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationResource](../resources/educationResource.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationResource.md)|
|originalFormId|String||
|viewUrl|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationFormResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationFormResource",
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
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": true,
  "viewUrl": "String",
  "editUrl": "String"
}
```

