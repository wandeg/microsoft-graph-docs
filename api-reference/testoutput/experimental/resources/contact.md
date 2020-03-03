---
title: "contact resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# contact resource type




Inherits from [outlookItem](../resources/outlookItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contact](../api/contact-get.md)|[contact](../resources/contact.md)|Read properties and relationships of the [contact](../resources/contact.md) object.|
|[Delete contact](../api/contact-delete.md)|None|Deletes a [contact](../resources/contact.md).|
|[Update contact](../api/contact-update.md)|[contact](../resources/contact.md)|Update the properties of a [contact](../resources/contact.md) object.|
|[List singleValueExtendedProperties](../api/contact-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/contact-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/contact-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/contact-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilePhoto.md)|Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.|
|[List extensions](../api/contact-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/contact-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assistantName|String||
|birthday|DateTimeOffset||
|categories|String collection| Inherited from [outlookItem](../resources/outlookItem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookItem.md)|
|children|String collection||
|companyName|String||
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookItem.md)|
|department|String||
|displayName|String||
|emailAddresses|[typedEmailAddress](../resources/typedEmailAddress.md) collection||
|fileAs|String||
|flag|[followupFlag](../resources/followupFlag.md)||
|gender|String||
|generation|String||
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|imAddresses|String collection||
|initials|String||
|isFavorite|Boolean||
|jobTitle|String||
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookItem.md)|
|manager|String||
|middleName|String||
|nickName|String||
|officeLocation|String||
|parentFolderId|String||
|personalNotes|String||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[physicalAddress](../resources/physicalAddress.md) collection||
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
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection||
|photo|[profilePhoto](../resources/profilePhoto.md)||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection||

## JSON Representation
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

