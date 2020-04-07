---
title: "educationSynchronizationCustomizations resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSynchronizationCustomizations resource type


Namespace: microsoft.graph




Inherits from [educationSynchronizationCustomizationsBase](../resources/educationsynchronizationcustomizationsbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|school|[educationSynchronizationCustomization](../resources/educationsynchronizationcustomization.md)||
|section|[educationSynchronizationCustomization](../resources/educationsynchronizationcustomization.md)||
|student|[educationSynchronizationCustomization](../resources/educationsynchronizationcustomization.md)||
|studentEnrollment|[educationSynchronizationCustomization](../resources/educationsynchronizationcustomization.md)||
|teacher|[educationSynchronizationCustomization](../resources/educationsynchronizationcustomization.md)||
|teacherRoster|[educationSynchronizationCustomization](../resources/educationsynchronizationcustomization.md)||

## Relationships
None

## JSON representation
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

