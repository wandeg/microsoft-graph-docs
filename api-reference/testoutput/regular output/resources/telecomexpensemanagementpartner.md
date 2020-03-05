---
title: "telecomExpenseManagementPartner resource type"
description: "telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service. Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# telecomExpenseManagementPartner resource type


Namespace: microsoft.graph

telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service. Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List telecomExpenseManagementPartners](../api/telecomexpensemanagementpartner-list.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) collection|List properties and relationships of the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) objects.|
|[Get telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Read properties and relationships of the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|
|[Create telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-create.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Create a new [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|
|[Delete telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-delete.md)|None|Deletes a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md).|
|[Update telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Update the properties of a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|
|[List telecomExpenseManagementPartners](../api/devicemanagement-list-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) collection|Get the telecomExpenseManagementPartners from the telecomExpenseManagementPartners navigation property.|
|[Add telecomExpenseManagementPartners](../api/devicemanagement-post-telecomexpensemanagementpartners.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Add telecomExpenseManagementPartners by posting to the telecomExpenseManagementPartners collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAuthorized|Boolean|Whether the partner's AAD app has been authorized to access Intune.|
|displayName|String|Display name of the TEM partner.|
|enabled|Boolean|Whether Intune's connection to the TEM service is currently enabled or disabled.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Timestamp of the last request sent to Intune by the TEM partner.|
|url|String|URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```

