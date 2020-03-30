---
title: "vppToken resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vppToken resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get vppToken](../api/vpptoken-get.md)|[vppToken](../resources/vpptoken.md)|Read properties and relationships of the [vppToken](../resources/vpptoken.md) object.|
|[Update vppToken](../api/vpptoken-update.md)|[vppToken](../resources/vpptoken.md)|Update the properties of a [vppToken](../resources/vpptoken.md) object.|
|[syncLicenses](../api/vpptoken-synclicenses.md)|[vppToken](../resources/vpptoken.md)||
|[revokeLicenses](../api/vpptoken-revokelicenses.md)|None||
|[getLicensesForApp](../api/vpptoken-getlicensesforapp.md)|[vppTokenLicenseSummary](../resources/vpptokenlicensesummary.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String||
|automaticallyUpdateApps|Boolean||
|claimTokenManagementFromExternalMdm|Boolean||
|countryOrRegion|String||
|dataSharingConsentGranted|Boolean||
|displayName|String||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|lastSyncStatus|Enumeration| Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|locationName|String||
|organizationName|String||
|roleScopeTagIds|String collection||
|state|Enumeration| Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|token|String||
|tokenActionResults|[vppTokenActionResult](../resources/vpptokenactionresult.md) collection||
|vppTokenAccountType|Enumeration| Possible values are: `business`, `education`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String",
  "dataSharingConsentGranted": true,
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```

