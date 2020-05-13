---
title: "vppToken resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vppToken resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List vppTokens](../api/intune-deviceappmanagement-list-vpptokens.md)|[vppToken](../resources/intune-vpptoken.md) collection|Get the vppTokens from the vppTokens navigation property.|
|[Create vppTokens](../api/intune-deviceappmanagement-post-vpptokens.md)|[vppToken](../resources/intune-vpptoken.md)|Create a new vppTokens object.|
|[Delete vppTokens](../api/intune-deviceappmanagement-delete-vpptokens.md)|None|Delete a [vppToken](../resources/intune-vpptoken.md) object.|
|[Update vppTokens](../api/intune-deviceappmanagement-update-vpptokens.md)|[vppToken](../resources/intune-vpptoken.md)|Update the properties of a vppTokens object.|
|[Get vppTokens](../api/intune-deviceappmanagement-get-vpptoken.md)|[vppToken](../resources/intune-vpptoken.md)|Read the properties and relationships of a [vppToken](../resources/intune-vpptoken.md) object.|
|[syncLicenses](../api/intune-vpptoken-synclicenses.md)|[vppToken](../resources/intune-vpptoken.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|**TODO: Add Description**|
|automaticallyUpdateApps|Boolean|**TODO: Add Description**|
|countryOrRegion|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncStatus|vppTokenSyncStatus|**TODO: Add Description**. Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|organizationName|String|**TODO: Add Description**|
|state|vppTokenState|**TODO: Add Description**. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|token|String|**TODO: Add Description**|
|vppTokenAccountType|vppTokenAccountType|**TODO: Add Description**. Possible values are: `business`, `education`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": "Boolean",
  "countryOrRegion": "String"
}
```

