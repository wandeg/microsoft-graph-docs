---
title: "educationPowerSchoolDataProvider resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationPowerSchoolDataProvider resource type


Namespace: microsoft.graph




Inherits from [educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowTeachersInMultipleSchools|Boolean||
|clientId|String||
|clientSecret|String||
|connectionUrl|String||
|customizations|[educationSynchronizationCustomizations](../resources/educationsynchronizationcustomizations.md)||
|schoolsIds|String collection||
|schoolYear|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": [
    "String"
  ],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": true,
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

