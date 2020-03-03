---
title: "educationCsvDataProvider resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationCsvDataProvider resource type




Inherits from [educationSynchronizationDataProvider](../resources/educationSynchronizationDataProvider.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customizations|[educationSynchronizationCustomizations](../resources/educationSynchronizationCustomizations.md)||

## Relationships
None

## JSON Representation
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

