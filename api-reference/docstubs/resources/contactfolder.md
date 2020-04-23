---
title: "contactFolder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# contactFolder resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contactFolder](../api/contactfolder-get.md)|[contactFolder](../resources/contactfolder.md)|Read the properties and relationships of a [contactFolder](../resources/contactfolder.md) object.|
|[Update contactFolder](../api/contactfolder-update.md)|[contactFolder](../resources/contactfolder.md)|Update the properties of a [contactFolder](../resources/contactfolder.md) object.|
|[delta](../api/contactfolder-delta.md)|[contactFolder](../resources/contactfolder.md) collection|**TODO: Add Description**|
|[List singleValueExtendedProperties](../api/contactfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/contactfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/contactfolder-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/contactfolder-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-get.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/contactfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/contactfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/contactfolder-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/contactfolder-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-get.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[List contacts](../api/contactfolder-list-contacts.md)|[contact](../resources/contact.md) collection|Get the contacts from the contacts navigation property.|
|[Create contacts](../api/contactfolder-post-contacts.md)|[contact](../resources/contact.md)|Create a new contacts object.|
|[Delete contacts](../api/contactfolder-delete-contacts.md)|None|Delete a [contact](../resources/contact.md) object.|
|[Update contacts](../api/contactfolder-update-contacts.md)|[contact](../resources/contact.md)|Update the properties of a contacts object.|
|[Get contact](../api/contact-get.md)|[contact](../resources/contact.md)|Read the properties and relationships of a [contact](../resources/contact.md) object.|
|[List childFolders](../api/contactfolder-list-childfolders.md)|[contactFolder](../resources/contactfolder.md) collection|Get the contactFolders from the childFolders navigation property.|
|[Create childFolders](../api/contactfolder-post-childfolders.md)|[contactFolder](../resources/contactfolder.md)|Create a new childFolders object.|
|[Delete childFolders](../api/contactfolder-delete-childfolders.md)|None|Delete a [contactFolder](../resources/contactfolder.md) object.|
|[Update childFolders](../api/contactfolder-update-childfolders.md)|[contactFolder](../resources/contactfolder.md)|Update the properties of a childFolders object.|
|[Get contactFolder](../api/contactfolder-get.md)|[contactFolder](../resources/contactfolder.md)|Read the properties and relationships of a [contactFolder](../resources/contactfolder.md) object.|
|[List childFolders](../api/contactfolder-list-childfolders.md)|[contactFolder](../resources/contactfolder.md) collection|Get the contactFolders from the childFolders navigation property.|
|[Create childFolders](../api/contactfolder-post-childfolders.md)|[contactFolder](../resources/contactfolder.md)|Create a new childFolders object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|parentFolderId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[contactFolder](../resources/contactfolder.md) collection|**TODO: Add Description**|
|contacts|[contact](../resources/contact.md) collection|**TODO: Add Description**|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contactFolder",
  "id": "String (identifier)",
  "parentFolderId": "String",
  "displayName": "String"
}
```

