---
title: "educationCsvDataProvider resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationCsvDataProvider resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customizations|[educationSynchronizationCustomizations](../resources/educationsynchronizationcustomizations.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationCsvDataProvider",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations",
    "school": {
      "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
      "optionalPropertiesToSync": [
        "String"
      ],
      "synchronizationStartDate": "String (timestamp)",
      "isSyncDeferred": true,
      "allowDisplayNameUpdate": true
    },
    "section": {
      "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
    },
    "student": {
      "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
    },
    "teacher": {
      "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
    },
    "studentEnrollment": {
      "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
    },
    "teacherRoster": {
      "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
    }
  }
}
```

