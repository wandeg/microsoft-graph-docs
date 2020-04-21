---
title: "educationStudent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# educationStudent resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|birthDate|Date|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|gender|educationGender|**TODO: Add Description**. Possible values are: `female`, `male`, `other`, `unknownFutureValue`.|
|grade|String|**TODO: Add Description**|
|graduationYear|String|**TODO: Add Description**|
|studentNumber|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "Date",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```

