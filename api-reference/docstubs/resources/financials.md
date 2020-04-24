---
title: "financials resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# financials resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get financials](../api/financials-get.md)|[financials](../resources/financials.md)|Read the properties and relationships of a [financials](../resources/financials.md) object.|
|[Update financials](../api/financials-update.md)|[financials](../resources/financials.md)|Update the properties of a [financials](../resources/financials.md) object.|
|[List companies](../api/financials-list-companies.md)|[company](../resources/company.md) collection|Get the companies from the companies navigation property.|
|[Create companies](../api/financials-post-companies.md)|[company](../resources/company.md)|Create a new companies object.|
|[Delete companies](../api/financials-delete-companies.md)|None|Delete a [company](../resources/company.md) object.|
|[Update companies](../api/financials-update-companies.md)|[company](../resources/company.md)|Update the properties of a companies object.|
|[Get company](../api/company-get.md)|[company](../resources/company.md)|Read the properties and relationships of a [company](../resources/company.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|companies|[company](../resources/company.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.financials",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.financials",
  "id": "String (identifier)"
}
```

