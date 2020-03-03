---
title: "userAccountInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userAccountInformation resource type




Inherits from [itemFacet](../resources/itemFacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userAccountInformation](../api/useraccountinformation-get.md)|[userAccountInformation](../resources/userAccountInformation.md)|Read properties and relationships of the [userAccountInformation](../resources/useraccountinformation.md) object.|
|[Delete userAccountInformation](../api/useraccountinformation-delete.md)|None|Deletes a [userAccountInformation](../resources/useraccountinformation.md).|
|[Update userAccountInformation](../api/useraccountinformation-update.md)|[userAccountInformation](../resources/userAccountInformation.md)|Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ageGroup|String||
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemFacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|countryCode|String||
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferenceData.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|preferredLanguageTag|[localeInfo](../resources/localeInfo.md)||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
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

