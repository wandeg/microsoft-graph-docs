---
title: "azureADLicenseUsage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# azureADLicenseUsage resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List azureADLicenseUsages](../api/azureadlicenseusage-list.md)|[azureADLicenseUsage](../resources/azureADLicenseUsage.md) collection|List properties and relationships of the [azureADLicenseUsage](../resources/azureadlicenseusage.md) objects.|
|[Get azureADLicenseUsage](../api/azureadlicenseusage-get.md)|[azureADLicenseUsage](../resources/azureADLicenseUsage.md)|Read properties and relationships of the [azureADLicenseUsage](../resources/azureadlicenseusage.md) object.|
|[Create azureADLicenseUsage](../api/azureadlicenseusage-create.md)|[azureADLicenseUsage](../resources/azureADLicenseUsage.md)|Create a new [azureADLicenseUsage](../resources/azureadlicenseusage.md) object.|
|[Delete azureADLicenseUsage](../api/azureadlicenseusage-delete.md)|None|Deletes a [azureADLicenseUsage](../resources/azureadlicenseusage.md).|
|[Update azureADLicenseUsage](../api/azureadlicenseusage-update.md)|[azureADLicenseUsage](../resources/azureADLicenseUsage.md)|Update the properties of a [azureADLicenseUsage](../resources/azureadlicenseusage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|licenseInfoDetails|[licenseInfoDetail](../resources/licenseInfoDetail.md) collection||
|snapshotDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.azureADLicenseUsage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADLicenseUsage",
  "id": "String (identifier)",
  "snapshotDateTime": "String (timestamp)",
  "licenseInfoDetails": [
    {
      "@odata.type": "microsoft.graph.licenseInfoDetail"
    }
  ]
}
```

