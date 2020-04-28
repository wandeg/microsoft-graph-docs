---
title: "applicationSignInDetailedSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# applicationSignInDetailedSummary resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get applicationSignInDetailedSummary](../api/microsoft.aad.reporting-applicationsignindetailedsummary-get.md)|[applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md)|Read properties and relationships of an [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object.|
|[Update applicationSignInDetailedSummary](../api/microsoft.aad.reporting-applicationsignindetailedsummary-update.md)|[applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md)|Update the properties of a [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregatedEventDateTime|DateTimeOffset|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|signInCount|Int64|**TODO: Add Description**|
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.applicationSignInDetailedSummary",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.applicationSignInDetailedSummary",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "status": {
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus"
  },
  "signInCount": 1024,
  "aggregatedEventDateTime": "String (timestamp)"
}
```

