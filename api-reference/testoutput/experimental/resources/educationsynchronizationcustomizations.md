---
title: "educationSynchronizationCustomizations resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationSynchronizationCustomizations resource type




Inherits from [educationSynchronizationCustomizationsBase](../resources/educationSynchronizationCustomizationsBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|school|[educationSynchronizationCustomization](../resources/educationSynchronizationCustomization.md)||
|section|[educationSynchronizationCustomization](../resources/educationSynchronizationCustomization.md)||
|student|[educationSynchronizationCustomization](../resources/educationSynchronizationCustomization.md)||
|studentEnrollment|[educationSynchronizationCustomization](../resources/educationSynchronizationCustomization.md)||
|teacher|[educationSynchronizationCustomization](../resources/educationSynchronizationCustomization.md)||
|teacherRoster|[educationSynchronizationCustomization](../resources/educationSynchronizationCustomization.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations",
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
```

