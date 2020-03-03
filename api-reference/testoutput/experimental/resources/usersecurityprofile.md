---
title: "userSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userSecurityProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userSecurityProfile](../api/usersecurityprofile-get.md)|[userSecurityProfile](../resources/userSecurityProfile.md)|Read properties and relationships of the [userSecurityProfile](../resources/usersecurityprofile.md) object.|
|[Delete userSecurityProfile](../api/usersecurityprofile-delete.md)|None|Deletes a [userSecurityProfile](../resources/usersecurityprofile.md).|
|[Update userSecurityProfile](../api/usersecurityprofile-update.md)|[userSecurityProfile](../resources/userSecurityProfile.md)|Update the properties of a [userSecurityProfile](../resources/usersecurityprofile.md) object.|
|[List userSecurityProfiles](../api/security-list-usersecurityprofiles.md)|[userSecurityProfile](../resources/userSecurityProfile.md) collection|Get the userSecurityProfiles from the userSecurityProfiles navigation property.|
|[Add userSecurityProfiles](../api/security-post-usersecurityprofiles.md)|[userSecurityProfile](../resources/userSecurityProfile.md)|Add userSecurityProfiles by posting to the userSecurityProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accounts|[userAccount](../resources/userAccount.md) collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|createdDateTime|DateTimeOffset||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|riskScore|String||
|tags|String collection||
|userPrincipalName|String||
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSecurityProfile",
  "id": "String (identifier)",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount"
    }
  ],
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "userPrincipalName": "String",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

