---
title: "organizationalBrandingLocalization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# organizationalBrandingLocalization resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List localizations](../api/organizationalbranding-list-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) collection|Get the organizationalBrandingLocalizations from the localizations navigation property.|
|[Create localizations](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Create a new localizations object.|
|[Update localizations](../api/organizationalbranding-update-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Update the properties of a localizations object.|
|[Get localizations](../api/organizationalbranding-get-organizationalbrandinglocalization.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Read the properties and relationships of an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.|
|[Delete localizations](../api/organizationalbranding-delete-localizations.md)|None|Delete an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.|
|[List organizationalBrandingLocalizations](../api/organizationalbrandinglocalization-list.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) collection|Get a list of the [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) objects and their properties.|
|[Create organizationalBrandingLocalization](../api/organizationalbrandinglocalization-create.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Create a new [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.|
|[Get organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Read the properties and relationships of an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.|
|[Update organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Update the properties of an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.|
|[Delete organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|None|Deletes an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|backgroundColor|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|backgroundImage|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|bannerLogo|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|signInPageText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|squareLogo|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|usernameHintText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingLocalization",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

