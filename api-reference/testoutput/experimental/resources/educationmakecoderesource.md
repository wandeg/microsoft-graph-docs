---
title: "educationMakeCodeResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationMakeCodeResource resource type




Inherits from [educationResource](../resources/educationResource.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [educationResource](../resources/educationResource.md)|
|createdDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationResource.md)|
|displayName|String| Inherited from [educationResource](../resources/educationResource.md)|
|hostWebUrl|String||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationResource](../resources/educationResource.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationResource](../resources/educationResource.md)|
|projectId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationMakeCodeResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationMakeCodeResource",
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
  "hostWebUrl": "String",
  "projectId": "String"
}
```

