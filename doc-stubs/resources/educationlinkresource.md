---
title: "educationLinkResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationLinkResource resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [educationResource](../resources/educationresource.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [educationResource](../resources/educationresource.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [educationResource](../resources/educationresource.md)|
|displayName|String|**TODO: Add Description** Inherited from [educationResource](../resources/educationresource.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [educationResource](../resources/educationresource.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [educationResource](../resources/educationresource.md)|
|link|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationLinkResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationLinkResource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "link": "String"
}
```

