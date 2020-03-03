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
|[List applicationSignInDetailedSummaries](../api/applicationsignindetailedsummary-list.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection|List properties and relationships of the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) objects.|
|[Get applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Read properties and relationships of the [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[Create applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-create.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Create a new [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[Delete applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-delete.md)|None|Deletes a [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md).|
|[Update applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-update.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Update the properties of a [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|

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

## JSON Representation
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

