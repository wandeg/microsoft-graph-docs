---
title: "printConnector resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printConnector resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printConnector](../api/printconnector-get.md)|[printConnector](../resources/printconnector.md)|Read properties and relationships of the [printConnector](../resources/printconnector.md) object.|
|[Update printConnector](../api/printconnector-update.md)|[printConnector](../resources/printconnector.md)|Update the properties of a [printConnector](../resources/printconnector.md) object.|
|[List connectors](../api/printer-list-connectors.md)|[printConnector](../resources/printconnector.md) collection|Get the printConnectors from the connectors navigation property.|
|[Create connectors](../api/printer-post-connectors.md)|[printConnector](../resources/printconnector.md)|Create connectors by posting to the connectors collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appVersion|String||
|deviceHealth|[deviceHealth](../resources/devicehealth.md)||
|fullyQualifiedDomainName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|location|[printerLocation](../resources/printerlocation.md)||
|name|String||
|operatingSystem|String||
|registeredDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "name": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {
    "@odata.type": "microsoft.graph.deviceHealth"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```

