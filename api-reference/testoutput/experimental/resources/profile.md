---
title: "profile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# profile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List profiles](../api/profile-list.md)|[profile](../resources/profile.md) collection|List properties and relationships of the [profile](../resources/profile.md) objects.|
|[Get profile](../api/profile-get.md)|[profile](../resources/profile.md)|Read properties and relationships of the [profile](../resources/profile.md) object.|
|[Create profile](../api/profile-create.md)|[profile](../resources/profile.md)|Create a new [profile](../resources/profile.md) object.|
|[Delete profile](../api/profile-delete.md)|None|Deletes a [profile](../resources/profile.md).|
|[Update profile](../api/profile-update.md)|[profile](../resources/profile.md)|Update the properties of a [profile](../resources/profile.md) object.|
|[List account](../api/profile-list-account.md)|[userAccountInformation](../resources/userAccountInformation.md) collection|Get the userAccountInformations from the account navigation property.|
|[Add account](../api/profile-post-account.md)|[userAccountInformation](../resources/userAccountInformation.md)|Add account by posting to the account collection.|
|[List anniversaries](../api/profile-list-anniversaries.md)|[personAnniversary](../resources/personAnniversary.md) collection|Get the personAnniversaries from the anniversaries navigation property.|
|[Add anniversaries](../api/profile-post-anniversaries.md)|[personAnniversary](../resources/personAnniversary.md)|Add anniversaries by posting to the anniversaries collection.|
|[List educationalActivities](../api/profile-list-educationalactivities.md)|[educationalActivity](../resources/educationalActivity.md) collection|Get the educationalActivities from the educationalActivities navigation property.|
|[Add educationalActivities](../api/profile-post-educationalactivities.md)|[educationalActivity](../resources/educationalActivity.md)|Add educationalActivities by posting to the educationalActivities collection.|
|[List emails](../api/profile-list-emails.md)|[itemEmail](../resources/itemEmail.md) collection|Get the itemEmails from the emails navigation property.|
|[Add emails](../api/profile-post-emails.md)|[itemEmail](../resources/itemEmail.md)|Add emails by posting to the emails collection.|
|[List interests](../api/profile-list-interests.md)|[personInterest](../resources/personInterest.md) collection|Get the personInterests from the interests navigation property.|
|[Add interests](../api/profile-post-interests.md)|[personInterest](../resources/personInterest.md)|Add interests by posting to the interests collection.|
|[List languages](../api/profile-list-languages.md)|[languageProficiency](../resources/languageProficiency.md) collection|Get the languageProficiencies from the languages navigation property.|
|[Add languages](../api/profile-post-languages.md)|[languageProficiency](../resources/languageProficiency.md)|Add languages by posting to the languages collection.|
|[List names](../api/profile-list-names.md)|[personName](../resources/personName.md) collection|Get the personNames from the names navigation property.|
|[Add names](../api/profile-post-names.md)|[personName](../resources/personName.md)|Add names by posting to the names collection.|
|[List phones](../api/profile-list-phones.md)|[itemPhone](../resources/itemPhone.md) collection|Get the itemPhones from the phones navigation property.|
|[Add phones](../api/profile-post-phones.md)|[itemPhone](../resources/itemPhone.md)|Add phones by posting to the phones collection.|
|[List positions](../api/profile-list-positions.md)|[workPosition](../resources/workPosition.md) collection|Get the workPositions from the positions navigation property.|
|[Add positions](../api/profile-post-positions.md)|[workPosition](../resources/workPosition.md)|Add positions by posting to the positions collection.|
|[List projects](../api/profile-list-projects.md)|[projectParticipation](../resources/projectParticipation.md) collection|Get the projectParticipations from the projects navigation property.|
|[Add projects](../api/profile-post-projects.md)|[projectParticipation](../resources/projectParticipation.md)|Add projects by posting to the projects collection.|
|[List skills](../api/profile-list-skills.md)|[skillProficiency](../resources/skillProficiency.md) collection|Get the skillProficiencies from the skills navigation property.|
|[Add skills](../api/profile-post-skills.md)|[skillProficiency](../resources/skillProficiency.md)|Add skills by posting to the skills collection.|
|[List webAccounts](../api/profile-list-webaccounts.md)|[webAccount](../resources/webAccount.md) collection|Get the webAccounts from the webAccounts navigation property.|
|[Add webAccounts](../api/profile-post-webaccounts.md)|[webAccount](../resources/webAccount.md)|Add webAccounts by posting to the webAccounts collection.|
|[List websites](../api/profile-list-websites.md)|[personWebsite](../resources/personWebsite.md) collection|Get the personWebsites from the websites navigation property.|
|[Add websites](../api/profile-post-websites.md)|[personWebsite](../resources/personWebsite.md)|Add websites by posting to the websites collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[userAccountInformation](../resources/userAccountInformation.md) collection||
|anniversaries|[personAnniversary](../resources/personAnniversary.md) collection||
|educationalActivities|[educationalActivity](../resources/educationalActivity.md) collection||
|emails|[itemEmail](../resources/itemEmail.md) collection||
|interests|[personInterest](../resources/personInterest.md) collection||
|languages|[languageProficiency](../resources/languageProficiency.md) collection||
|names|[personName](../resources/personName.md) collection||
|phones|[itemPhone](../resources/itemPhone.md) collection||
|positions|[workPosition](../resources/workPosition.md) collection||
|projects|[projectParticipation](../resources/projectParticipation.md) collection||
|skills|[skillProficiency](../resources/skillProficiency.md) collection||
|webAccounts|[webAccount](../resources/webAccount.md) collection||
|websites|[personWebsite](../resources/personWebsite.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

