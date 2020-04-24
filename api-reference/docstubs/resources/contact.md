---
title: "contact resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# contact resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [outlookItem](../resources/outlookitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contact](../api/contact-get.md)|[contact](../resources/contact.md)|Read the properties and relationships of a [contact](../resources/contact.md) object.|
|[Update contact](../api/contact-update.md)|[contact](../resources/contact.md)|Update the properties of a [contact](../resources/contact.md) object.|
|[delta](../api/contact-delta.md)|[contact](../resources/contact.md) collection|**TODO: Add Description**|
|[List singleValueExtendedProperties](../api/contact-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/contact-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/contact-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/contact-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-get.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/contact-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/contact-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/contact-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/contact-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-get.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[List photo](../api/contact-list-photo.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photo navigation property.|
|[Create photo](../api/contact-post-photo.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photo object.|
|[Delete photo](../api/contact-delete-photo.md)|None|Delete a [profilePhoto](../resources/profilephoto.md) object.|
|[Update photo](../api/contact-update-photo.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a photo object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read the properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[List extensions](../api/contact-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/contact-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[Delete extensions](../api/contact-delete-extensions.md)|None|Delete an [extension](../resources/extension.md) object.|
|[Update extensions](../api/contact-update-extensions.md)|[extension](../resources/extension.md)|Update the properties of an extensions object.|
|[Get extension](../api/extension-get.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assistantName|String|**TODO: Add Description**|
|birthday|DateTimeOffset|**TODO: Add Description**|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|children|String collection|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|emailAddresses|[typedEmailAddress](../resources/typedemailaddress.md) collection|**TODO: Add Description**|
|fileAs|String|**TODO: Add Description**|
|flag|[followupFlag](../resources/followupflag.md)|**TODO: Add Description**|
|gender|String|**TODO: Add Description**|
|generation|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|imAddresses|String collection|**TODO: Add Description**|
|initials|String|**TODO: Add Description**|
|isFavorite|Boolean|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|manager|String|**TODO: Add Description**|
|middleName|String|**TODO: Add Description**|
|nickName|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description**|
|personalNotes|String|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|postalAddresses|[physicalAddress](../resources/physicaladdress.md) collection|**TODO: Add Description**|
|profession|String|**TODO: Add Description**|
|spouseName|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|websites|[website](../resources/website.md) collection|**TODO: Add Description**|
|weddingAnniversary|Date|**TODO: Add Description**|
|yomiCompanyName|String|**TODO: Add Description**|
|yomiGivenName|String|**TODO: Add Description**|
|yomiSurname|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|photo|[profilePhoto](../resources/profilephoto.md)|**TODO: Add Description**|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contact",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "parentFolderId": "String",
  "birthday": "String (timestamp)",
  "fileAs": "String",
  "displayName": "String",
  "givenName": "String",
  "initials": "String",
  "middleName": "String",
  "nickName": "String",
  "surname": "String",
  "title": "String",
  "yomiGivenName": "String",
  "yomiSurname": "String",
  "yomiCompanyName": "String",
  "generation": "String",
  "emailAddresses": [
    {
      "@odata.type": "microsoft.graph.typedEmailAddress",
      "name": "String",
      "address": "String",
      "type": "String",
      "otherLabel": "String"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website",
      "type": "String"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "jobTitle": "String",
  "companyName": "String",
  "department": "String",
  "officeLocation": "String",
  "profession": "String",
  "assistantName": "String",
  "manager": "String",
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
      "type": "String",
      "number": "String"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "String",
      "street": "String",
      "city": "String",
      "state": "String",
      "countryOrRegion": "String",
      "postalCode": "String"
    }
  ],
  "spouseName": "String",
  "personalNotes": "String",
  "children": [
    "String"
  ],
  "weddingAnniversary": "Date",
  "gender": "String",
  "isFavorite": true,
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "flagStatus": "String"
  }
}
```

