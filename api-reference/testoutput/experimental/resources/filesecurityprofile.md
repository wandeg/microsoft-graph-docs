---
title: "fileSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# fileSecurityProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get fileSecurityProfile](../api/filesecurityprofile-get.md)|[fileSecurityProfile](../resources/fileSecurityProfile.md)|Read properties and relationships of the [fileSecurityProfile](../resources/filesecurityprofile.md) object.|
|[Delete fileSecurityProfile](../api/filesecurityprofile-delete.md)|None|Deletes a [fileSecurityProfile](../resources/filesecurityprofile.md).|
|[Update fileSecurityProfile](../api/filesecurityprofile-update.md)|[fileSecurityProfile](../resources/fileSecurityProfile.md)|Update the properties of a [fileSecurityProfile](../resources/filesecurityprofile.md) object.|
|[List fileSecurityProfiles](../api/security-list-filesecurityprofiles.md)|[fileSecurityProfile](../resources/fileSecurityProfile.md) collection|Get the fileSecurityProfiles from the fileSecurityProfiles navigation property.|
|[Add fileSecurityProfiles](../api/security-post-filesecurityprofiles.md)|[fileSecurityProfile](../resources/fileSecurityProfile.md)|Add fileSecurityProfiles by posting to the fileSecurityProfiles collection.|

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
|hashes|[fileHash](../resources/fileHash.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSeenDateTime|DateTimeOffset||
|malwareStates|[malwareState](../resources/malwareState.md) collection||
|names|String collection||
|riskScore|String||
|size|Int64||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilityState.md) collection||

## Relationships
None

## JSON Representation
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

