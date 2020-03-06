---
title: "contact resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# contact resource type


Namespace: microsoft.graph




Inherits from [outlookItem](../resources/outlookitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contact](../api/contact-get.md)|[contact](../resources/contact.md)|Read properties and relationships of the [contact](../resources/contact.md) object.|
|[Update contact](../api/contact-update.md)|[contact](../resources/contact.md)|Update the properties of a [contact](../resources/contact.md) object.|
|[delta](../api/contact-delta.md)|[contact](../resources/contact.md) collection||
|[List singleValueExtendedProperties](../api/contact-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/contact-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/contact-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/contact-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.|
|[List extensions](../api/contact-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/contact-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List contacts](../api/contactfolder-list-contacts.md)|[contact](../resources/contact.md) collection|Get the contacts from the contacts navigation property.|
|[Add contacts](../api/contactfolder-post-contacts.md)|[contact](../resources/contact.md)|Add contacts by posting to the contacts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assistantName|String||
|birthday|DateTimeOffset||
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|children|String collection||
|companyName|String||
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|department|String||
|displayName|String||
|emailAddresses|[typedEmailAddress](../resources/typedemailaddress.md) collection||
|fileAs|String||
|flag|[followupFlag](../resources/followupflag.md)||
|gender|String||
|generation|String||
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|imAddresses|String collection||
|initials|String||
|isFavorite|Boolean||
|jobTitle|String||
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|manager|String||
|middleName|String||
|nickName|String||
|officeLocation|String||
|parentFolderId|String||
|personalNotes|String||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[physicalAddress](../resources/physicaladdress.md) collection||
|profession|String||
|spouseName|String||
|surname|String||
|title|String||
|websites|[website](../resources/website.md) collection||
|weddingAnniversary|Date||
|yomiCompanyName|String||
|yomiGivenName|String||
|yomiSurname|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|extensions|[extension](../resources/extension.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|photo|[profilePhoto](../resources/profilephoto.md)||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

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

