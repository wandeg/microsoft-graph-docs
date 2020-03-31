---
title: "applicationSignInDetailedSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# applicationSignInDetailedSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Read properties and relationships of the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[Update applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-update.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Update the properties of a [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[List applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection|Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property.|
|[Add applicationSignInDetailedSummary](../api/reportroot-post-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Add applicationSignInDetailedSummary by posting to the applicationSignInDetailedSummary collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregatedEventDateTime|DateTimeOffset||
|appDisplayName|String||
|appId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|signInCount|Int64||
|status|[signInStatus](../resources/signinstatus.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationSignInDetailedSummary",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "signInCount": 1024,
  "aggregatedEventDateTime": "String (timestamp)"
}
```

