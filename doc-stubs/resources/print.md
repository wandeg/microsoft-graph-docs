---
title: "print resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# print resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get print](../api/print-get.md)|[print](../resources/print.md)|Read the properties and relationships of a [print](../resources/print.md) object.|
|[Update print](../api/print-update.md)|[print](../resources/print.md)|Update the properties of a [print](../resources/print.md) object.|
|[List services](../api/print-list-services.md)|[printService](../resources/printservice.md) collection|Get the printServices from the services navigation property.|
|[Create services](../api/print-post-services.md)|[printService](../resources/printservice.md)|Create a new services object.|
|[Delete services](../api/print-delete-services.md)|None|Delete a [printService](../resources/printservice.md) object.|
|[Update services](../api/print-update-services.md)|[printService](../resources/printservice.md)|Update the properties of a services object.|
|[Get printService](../api/printservice-get.md)|[printService](../resources/printservice.md)|Read the properties and relationships of a [printService](../resources/printservice.md) object.|
|[List printers](../api/print-list-printers.md)|[printer](../resources/printer.md) collection|Get the printers from the printers navigation property.|
|[Create printers](../api/print-post-printers.md)|[printer](../resources/printer.md)|Create a new printers object.|
|[Delete printers](../api/print-delete-printers.md)|None|Delete a [printer](../resources/printer.md) object.|
|[Update printers](../api/print-update-printers.md)|[printer](../resources/printer.md)|Update the properties of a printers object.|
|[Get printer](../api/printer-get.md)|[printer](../resources/printer.md)|Read the properties and relationships of a [printer](../resources/printer.md) object.|
|[List connectors](../api/print-list-connectors.md)|[printConnector](../resources/printconnector.md) collection|Get the printConnectors from the connectors navigation property.|
|[Create connectors](../api/print-post-connectors.md)|[printConnector](../resources/printconnector.md)|Create a new connectors object.|
|[Delete connectors](../api/print-delete-connectors.md)|None|Delete a [printConnector](../resources/printconnector.md) object.|
|[Update connectors](../api/print-update-connectors.md)|[printConnector](../resources/printconnector.md)|Update the properties of a connectors object.|
|[Get printConnector](../api/printconnector-get.md)|[printConnector](../resources/printconnector.md)|Read the properties and relationships of a [printConnector](../resources/printconnector.md) object.|
|[List shares](../api/print-list-shares.md)|[printerShare](../resources/printershare.md) collection|Get the printerShares from the shares navigation property.|
|[Create shares](../api/print-post-shares.md)|[printerShare](../resources/printershare.md)|Create a new shares object.|
|[Delete shares](../api/print-delete-shares.md)|None|Delete a [printerShare](../resources/printershare.md) object.|
|[Update shares](../api/print-update-shares.md)|[printerShare](../resources/printershare.md)|Update the properties of a shares object.|
|[Get printerShare](../api/printershare-get.md)|[printerShare](../resources/printershare.md)|Read the properties and relationships of a [printerShare](../resources/printershare.md) object.|
|[List printerShares](../api/print-list-printershares.md)|[printerShare](../resources/printershare.md) collection|Get the printerShares from the printerShares navigation property.|
|[Create printerShares](../api/print-post-printershares.md)|[printerShare](../resources/printershare.md)|Create a new printerShares object.|
|[Delete printerShares](../api/print-delete-printershares.md)|None|Delete a [printerShare](../resources/printershare.md) object.|
|[Update printerShares](../api/print-update-printershares.md)|[printerShare](../resources/printershare.md)|Update the properties of a printerShares object.|
|[Get printerShare](../api/printershare-get.md)|[printerShare](../resources/printershare.md)|Read the properties and relationships of a [printerShare](../resources/printershare.md) object.|
|[List reports](../api/print-list-reports.md)|[reportRoot](../resources/reportroot.md) collection|Get the reportRoots from the reports navigation property.|
|[Create reports](../api/print-post-reports.md)|[reportRoot](../resources/reportroot.md)|Create a new reports object.|
|[Delete reports](../api/print-delete-reports.md)|None|Delete a [reportRoot](../resources/reportroot.md) object.|
|[Update reports](../api/print-update-reports.md)|[reportRoot](../resources/reportroot.md)|Update the properties of a reports object.|
|[Get reportRoot](../api/reportroot-get.md)|[reportRoot](../resources/reportroot.md)|Read the properties and relationships of a [reportRoot](../resources/reportroot.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settings|[printSettings](../resources/printsettings.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connectors|[printConnector](../resources/printconnector.md) collection|**TODO: Add Description**|
|printers|[printer](../resources/printer.md) collection|**TODO: Add Description**|
|printerShares|[printerShare](../resources/printershare.md) collection|**TODO: Add Description**|
|reports|[reportRoot](../resources/reportroot.md) collection|**TODO: Add Description**|
|services|[printService](../resources/printservice.md) collection|**TODO: Add Description**|
|shares|[printerShare](../resources/printershare.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

