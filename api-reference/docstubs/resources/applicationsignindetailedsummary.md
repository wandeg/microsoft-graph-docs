---
title: "applicationSignInDetailedSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applicationSignInDetailedSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Read the properties and relationships of an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[Update applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-update.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Update the properties of an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[List applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection|Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property.|
|[Create applicationSignInDetailedSummary](../api/reportroot-post-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Create a new applicationSignInDetailedSummary object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregatedEventDateTime|DateTimeOffset|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|signInCount|Int64|**TODO: Add Description**|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description**|

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

