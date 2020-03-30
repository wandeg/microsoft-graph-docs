---
title: "print resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# print resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get print](../api/print-get.md)|[print](../resources/print.md)|Read properties and relationships of the [print](../resources/print.md) object.|
|[Update print](../api/print-update.md)|[print](../resources/print.md)|Update the properties of a [print](../resources/print.md) object.|
|[List services](../api/print-list-services.md)|[printService](../resources/printservice.md) collection|Get the printServices from the services navigation property.|
|[Add services](../api/print-post-services.md)|[printService](../resources/printservice.md)|Add services by posting to the services collection.|
|[List printers](../api/print-list-printers.md)|[printer](../resources/printer.md) collection|Get the printers from the printers navigation property.|
|[Add printers](../api/print-post-printers.md)|[printer](../resources/printer.md)|Add printers by posting to the printers collection.|
|[List connectors](../api/print-list-connectors.md)|[printConnector](../resources/printconnector.md) collection|Get the printConnectors from the connectors navigation property.|
|[Add connectors](../api/print-post-connectors.md)|[printConnector](../resources/printconnector.md)|Add connectors by posting to the connectors collection.|
|[List printerShares](../api/print-list-printershares.md)|[printerShare](../resources/printershare.md) collection|Get the printerShares from the printerShares navigation property.|
|[Add printerShares](../api/print-post-printershares.md)|[printerShare](../resources/printershare.md)|Add printerShares by posting to the printerShares collection.|
|[List reports](../api/print-list-reports.md)|[reportRoot](../resources/reportroot.md) collection|Get the reportRoots from the reports navigation property.|
|[Add reports](../api/print-post-reports.md)|[reportRoot](../resources/reportroot.md)|Add reports by posting to the reports collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settings|[printSettings](../resources/printsettings.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connectors|[printConnector](../resources/printconnector.md) collection||
|printers|[printer](../resources/printer.md) collection||
|printerShares|[printerShare](../resources/printershare.md) collection||
|reports|[reportRoot](../resources/reportroot.md) collection||
|services|[printService](../resources/printservice.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings",
    "documentConversionEnabled": true
  }
}
```

