---
title: "userAccountInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userAccountInformation resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userAccountInformation](../api/useraccountinformation-get.md)|[userAccountInformation](../resources/useraccountinformation.md)|Read properties and relationships of the [userAccountInformation](../resources/useraccountinformation.md) object.|
|[Update userAccountInformation](../api/useraccountinformation-update.md)|[userAccountInformation](../resources/useraccountinformation.md)|Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.|
|[List account](../api/profile-list-account.md)|[userAccountInformation](../resources/useraccountinformation.md) collection|Get the userAccountInformations from the account navigation property.|
|[Add account](../api/profile-post-account.md)|[userAccountInformation](../resources/useraccountinformation.md)|Add account by posting to the account collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ageGroup|String||
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|countryCode|String||
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|preferredLanguageTag|[localeInfo](../resources/localeinfo.md)||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```

