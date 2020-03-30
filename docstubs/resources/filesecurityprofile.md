---
title: "fileSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileSecurityProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get fileSecurityProfile](../api/filesecurityprofile-get.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Read properties and relationships of the [fileSecurityProfile](../resources/filesecurityprofile.md) object.|
|[Update fileSecurityProfile](../api/filesecurityprofile-update.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Update the properties of a [fileSecurityProfile](../resources/filesecurityprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|certificateThumbprint|String||
|extensions|String collection||
|fileType|String||
|firstSeenDateTime|DateTimeOffset||
|hashes|[fileHash](../resources/filehash.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSeenDateTime|DateTimeOffset||
|malwareStates|[malwareState](../resources/malwarestate.md) collection||
|names|String collection||
|riskScore|String||
|size|Int64||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fileSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileSecurityProfile",
  "id": "String (identifier)",
  "activityGroupNames": [
    "String"
  ],
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "certificateThumbprint": "String",
  "extensions": [
    "String"
  ],
  "fileType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash"
    }
  ],
  "lastSeenDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState"
    }
  ],
  "names": [
    "String"
  ],
  "riskScore": "String",
  "size": 1024,
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState"
    }
  ]
}
```

