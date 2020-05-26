---
title: "profile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# profile resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List profiles](../api/profile-list.md)|[profile](../resources/profile.md) collection|Get a list of the [profile](../resources/profile.md) objects and their properties.|
|[Create profile](../api/profile-create.md)|[profile](../resources/profile.md)|Create a new [profile](../resources/profile.md) object.|
|[Get profile](../api/profile-get.md)|[profile](../resources/profile.md)|Read the properties and relationships of a [profile](../resources/profile.md) object.|
|[Update profile](../api/profile-update.md)|[profile](../resources/profile.md)|Update the properties of a [profile](../resources/profile.md) object.|
|[Delete profile](../api/profile-delete.md)|None|Deletes a [profile](../resources/profile.md) object.|
|[List addresses](../api/profile-list-addresses.md)|[itemAddress](../resources/itemaddress.md) collection|Get the itemAddresses from the addresses navigation property.|
|[Create addresses](../api/profile-post-addresses.md)|[itemAddress](../resources/itemaddress.md)|Create a new addresses object.|
|[Get addresses](../api/profile-get-itemaddress.md)|[itemAddress](../resources/itemaddress.md)|Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.|
|[Update addresses](../api/profile-update-addresses.md)|[itemAddress](../resources/itemaddress.md)|Update the properties of an addresses object.|
|[Delete addresses](../api/profile-delete-addresses.md)|None|Delete an [itemAddress](../resources/itemaddress.md) object.|
|[List notes](../api/profile-list-notes.md)|[personAnnotation](../resources/personannotation.md) collection|Get the personAnnotations from the notes navigation property.|
|[Create notes](../api/profile-post-notes.md)|[personAnnotation](../resources/personannotation.md)|Create a new notes object.|
|[Get notes](../api/profile-get-personannotation.md)|[personAnnotation](../resources/personannotation.md)|Read the properties and relationships of a [personAnnotation](../resources/personannotation.md) object.|
|[Update notes](../api/profile-update-notes.md)|[personAnnotation](../resources/personannotation.md)|Update the properties of a notes object.|
|[Delete notes](../api/profile-delete-notes.md)|None|Delete a [personAnnotation](../resources/personannotation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[userAccountInformation](../resources/useraccountinformation.md) collection|**TODO: Add Description**|
|addresses|[itemAddress](../resources/itemaddress.md) collection|**TODO: Add Description**|
|anniversaries|[personAnniversary](../resources/personanniversary.md) collection|**TODO: Add Description**|
|educationalActivities|[educationalActivity](../resources/educationalactivity.md) collection|**TODO: Add Description**|
|emails|[itemEmail](../resources/itememail.md) collection|**TODO: Add Description**|
|interests|[personInterest](../resources/personinterest.md) collection|**TODO: Add Description**|
|languages|[languageProficiency](../resources/languageproficiency.md) collection|**TODO: Add Description**|
|names|[personName](../resources/personname.md) collection|**TODO: Add Description**|
|notes|[personAnnotation](../resources/personannotation.md) collection|**TODO: Add Description**|
|phones|[itemPhone](../resources/itemphone.md) collection|**TODO: Add Description**|
|positions|[workPosition](../resources/workposition.md) collection|**TODO: Add Description**|
|projects|[projectParticipation](../resources/projectparticipation.md) collection|**TODO: Add Description**|
|skills|[skillProficiency](../resources/skillproficiency.md) collection|**TODO: Add Description**|
|webAccounts|[webAccount](../resources/webaccount.md) collection|**TODO: Add Description**|
|websites|[personWebsite](../resources/personwebsite.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.profile",
  "id": "String (identifier)"
}
```

