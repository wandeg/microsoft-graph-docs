---
title: "profile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# profile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get profile](../api/profile-get.md)|[profile](../resources/profile.md)|Read properties and relationships of the [profile](../resources/profile.md) object.|
|[Update profile](../api/profile-update.md)|[profile](../resources/profile.md)|Update the properties of a [profile](../resources/profile.md) object.|
|[List account](../api/profile-list-account.md)|[userAccountInformation](../resources/useraccountinformation.md) collection|Get the userAccountInformations from the account navigation property.|
|[Add account](../api/profile-post-account.md)|[userAccountInformation](../resources/useraccountinformation.md)|Add account by posting to the account collection.|
|[List anniversaries](../api/profile-list-anniversaries.md)|[personAnniversary](../resources/personanniversary.md) collection|Get the personAnniversaries from the anniversaries navigation property.|
|[Add anniversaries](../api/profile-post-anniversaries.md)|[personAnniversary](../resources/personanniversary.md)|Add anniversaries by posting to the anniversaries collection.|
|[List educationalActivities](../api/profile-list-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md) collection|Get the educationalActivities from the educationalActivities navigation property.|
|[Add educationalActivities](../api/profile-post-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md)|Add educationalActivities by posting to the educationalActivities collection.|
|[List emails](../api/profile-list-emails.md)|[itemEmail](../resources/itememail.md) collection|Get the itemEmails from the emails navigation property.|
|[Add emails](../api/profile-post-emails.md)|[itemEmail](../resources/itememail.md)|Add emails by posting to the emails collection.|
|[List interests](../api/profile-list-interests.md)|[personInterest](../resources/personinterest.md) collection|Get the personInterests from the interests navigation property.|
|[Add interests](../api/profile-post-interests.md)|[personInterest](../resources/personinterest.md)|Add interests by posting to the interests collection.|
|[List languages](../api/profile-list-languages.md)|[languageProficiency](../resources/languageproficiency.md) collection|Get the languageProficiencies from the languages navigation property.|
|[Add languages](../api/profile-post-languages.md)|[languageProficiency](../resources/languageproficiency.md)|Add languages by posting to the languages collection.|
|[List names](../api/profile-list-names.md)|[personName](../resources/personname.md) collection|Get the personNames from the names navigation property.|
|[Add names](../api/profile-post-names.md)|[personName](../resources/personname.md)|Add names by posting to the names collection.|
|[List phones](../api/profile-list-phones.md)|[itemPhone](../resources/itemphone.md) collection|Get the itemPhones from the phones navigation property.|
|[Add phones](../api/profile-post-phones.md)|[itemPhone](../resources/itemphone.md)|Add phones by posting to the phones collection.|
|[List positions](../api/profile-list-positions.md)|[workPosition](../resources/workposition.md) collection|Get the workPositions from the positions navigation property.|
|[Add positions](../api/profile-post-positions.md)|[workPosition](../resources/workposition.md)|Add positions by posting to the positions collection.|
|[List projects](../api/profile-list-projects.md)|[projectParticipation](../resources/projectparticipation.md) collection|Get the projectParticipations from the projects navigation property.|
|[Add projects](../api/profile-post-projects.md)|[projectParticipation](../resources/projectparticipation.md)|Add projects by posting to the projects collection.|
|[List skills](../api/profile-list-skills.md)|[skillProficiency](../resources/skillproficiency.md) collection|Get the skillProficiencies from the skills navigation property.|
|[Add skills](../api/profile-post-skills.md)|[skillProficiency](../resources/skillproficiency.md)|Add skills by posting to the skills collection.|
|[List webAccounts](../api/profile-list-webaccounts.md)|[webAccount](../resources/webaccount.md) collection|Get the webAccounts from the webAccounts navigation property.|
|[Add webAccounts](../api/profile-post-webaccounts.md)|[webAccount](../resources/webaccount.md)|Add webAccounts by posting to the webAccounts collection.|
|[List websites](../api/profile-list-websites.md)|[personWebsite](../resources/personwebsite.md) collection|Get the personWebsites from the websites navigation property.|
|[Add websites](../api/profile-post-websites.md)|[personWebsite](../resources/personwebsite.md)|Add websites by posting to the websites collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[userAccountInformation](../resources/useraccountinformation.md) collection||
|anniversaries|[personAnniversary](../resources/personanniversary.md) collection||
|educationalActivities|[educationalActivity](../resources/educationalactivity.md) collection||
|emails|[itemEmail](../resources/itememail.md) collection||
|interests|[personInterest](../resources/personinterest.md) collection||
|languages|[languageProficiency](../resources/languageproficiency.md) collection||
|names|[personName](../resources/personname.md) collection||
|phones|[itemPhone](../resources/itemphone.md) collection||
|positions|[workPosition](../resources/workposition.md) collection||
|projects|[projectParticipation](../resources/projectparticipation.md) collection||
|skills|[skillProficiency](../resources/skillproficiency.md) collection||
|webAccounts|[webAccount](../resources/webaccount.md) collection||
|websites|[personWebsite](../resources/personwebsite.md) collection||

## JSON representation
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

