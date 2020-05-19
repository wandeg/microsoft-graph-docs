---
title: "LIMember resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMember resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certifications|[LIMemberCertification](../resources/limembercertification.md) collection|**TODO: Add Description**|
|connectionInfo|[LIMemberConnectionInfo](../resources/limemberconnectioninfo.md)|**TODO: Add Description**|
|defaultLocale|[Locale](../resources/locale.md)|**TODO: Add Description**|
|educations|[LIMemberEducation](../resources/limembereducation.md) collection|**TODO: Add Description**|
|emails|String collection|**TODO: Add Description**|
|firstName|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|headline|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|honors|[LIMemberHonor](../resources/limemberhonor.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|industryName|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|invitation|[LIInvite](../resources/liinvite.md)|**TODO: Add Description**|
|languages|[LIMemberLanguage](../resources/limemberlanguage.md) collection|**TODO: Add Description**|
|lastName|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|location|[LILocation](../resources/lilocation.md)|**TODO: Add Description**|
|mutualConnections|[LIMutualConnections](../resources/limutualconnections.md)|**TODO: Add Description**|
|organizations|[LIMemberOrganization](../resources/limemberorganization.md) collection|**TODO: Add Description**|
|patents|[LIMemberPatent](../resources/limemberpatent.md) collection|**TODO: Add Description**|
|positions|[LIMemberPosition](../resources/limemberposition.md) collection|**TODO: Add Description**|
|profilePicture|String|**TODO: Add Description**|
|profileUrl|String|**TODO: Add Description**|
|projects|[LIMemberProject](../resources/limemberproject.md) collection|**TODO: Add Description**|
|publications|[LIMemberPublication](../resources/limemberpublication.md) collection|**TODO: Add Description**|
|skills|[LISkill](../resources/liskill.md) collection|**TODO: Add Description**|
|summary|[MultiLocaleRichText](../resources/multilocalerichtext.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMember"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMember",
  "mutualConnections": {
    "@odata.type": "microsoft.graph.LIMutualConnections"
  },
  "invitation": {
    "@odata.type": "microsoft.graph.LIInvite"
  },
  "id": "String (identifier)",
  "firstName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "lastName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "headline": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "summary": {
    "@odata.type": "microsoft.graph.MultiLocaleRichText"
  },
  "industryName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "profilePicture": "String",
  "defaultLocale": {
    "@odata.type": "microsoft.graph.Locale"
  },
  "profileUrl": "String",
  "positions": [
    {
      "@odata.type": "microsoft.graph.LIMemberPosition"
    }
  ],
  "educations": [
    {
      "@odata.type": "microsoft.graph.LIMemberEducation"
    }
  ],
  "certifications": [
    {
      "@odata.type": "microsoft.graph.LIMemberCertification"
    }
  ],
  "honors": [
    {
      "@odata.type": "microsoft.graph.LIMemberHonor"
    }
  ],
  "languages": [
    {
      "@odata.type": "microsoft.graph.LIMemberLanguage"
    }
  ],
  "organizations": [
    {
      "@odata.type": "microsoft.graph.LIMemberOrganization"
    }
  ],
  "patents": [
    {
      "@odata.type": "microsoft.graph.LIMemberPatent"
    }
  ],
  "projects": [
    {
      "@odata.type": "microsoft.graph.LIMemberProject"
    }
  ],
  "publications": [
    {
      "@odata.type": "microsoft.graph.LIMemberPublication"
    }
  ],
  "skills": [
    {
      "@odata.type": "microsoft.graph.LISkill"
    }
  ],
  "emails": [
    "String"
  ],
  "connectionInfo": {
    "@odata.type": "microsoft.graph.LIMemberConnectionInfo"
  },
  "location": {
    "@odata.type": "microsoft.graph.LILocation"
  }
}
```

