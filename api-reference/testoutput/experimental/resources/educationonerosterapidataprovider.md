---
title: "educationOneRosterApiDataProvider resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationOneRosterApiDataProvider resource type


Namespace: microsoft.graph




Inherits from [educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|connectionSettings|[educationSynchronizationConnectionSettings](../resources/educationsynchronizationconnectionsettings.md)||
|connectionUrl|String||
|customizations|[educationSynchronizationCustomizations](../resources/educationsynchronizationcustomizations.md)||
|providerName|String||
|schoolsIds|String collection||
|termIds|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOneRosterApiDataProvider"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationOneRosterApiDataProvider",
  "connectionUrl": "String",
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "schoolsIds": [
    "String"
  ],
  "termIds": [
    "String"
  ],
  "providerName": "String",
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

