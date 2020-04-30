---
title: "orgContact resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# orgContact resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List orgContacts](../api/microsoft.directoryservices-orgcontact-list.md)|[orgContact](../resources/microsoft.directoryservices-orgcontact.md) collection|Get a list of the [orgContact](../resources/orgcontact.md) objects and their properties.|
|[Get orgContact](../api/microsoft.directoryservices-orgcontact-get.md)|[orgContact](../resources/microsoft.directoryservices-orgcontact.md)|Read properties and relationships of an [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object.|
|[Create orgContact](../api/microsoft.directoryservices-orgcontact-post-contacts.md)|[orgContact](../resources/microsoft.directoryservices-orgcontact.md)|Create a new [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object.|
|[Delete orgContact](../api/microsoft.directoryservices-orgcontact-delete.md)|None|Deletes an [orgContact](../resources/microsoft.directoryservices-orgcontact.md).|
|[Update orgContact](../api/microsoft.directoryservices-orgcontact-update.md)|[orgContact](../resources/microsoft.directoryservices-orgcontact.md)|Update the properties of a [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object.|
|[delta](../api/microsoft.directoryservices-orgcontact-delta.md)|[orgContact](../resources/microsoft.directoryservices-orgcontact.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/microsoft.directoryservices-orgcontact-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-orgcontact-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-orgcontact-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-orgcontact-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-orgcontact-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[List manager](../api/microsoft.directoryservices-orgcontact-list-manager.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the manager navigation property.|
|[Add manager](../api/microsoft.directoryservices-orgcontact-post-manager.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add manager by posting to the manager collection.|
|[Remove manager](../api/microsoft.directoryservices-orgcontact-delete-manager.md)|None|Remove a manager object.|
|[List directReports](../api/microsoft.directoryservices-orgcontact-list-directreports.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the directReports navigation property.|
|[Add directReports](../api/microsoft.directoryservices-orgcontact-post-directreports.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add directReports by posting to the directReports collection.|
|[Remove directReports](../api/microsoft.directoryservices-orgcontact-delete-directreports.md)|None|Remove a directReports object.|
|[List memberOf](../api/microsoft.directoryservices-orgcontact-list-memberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/microsoft.directoryservices-orgcontact-post-memberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/microsoft.directoryservices-orgcontact-delete-memberof.md)|None|Remove a memberOf object.|
|[List transitiveMemberOf](../api/microsoft.directoryservices-orgcontact-list-transitivememberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/microsoft.directoryservices-orgcontact-post-transitivememberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/microsoft.directoryservices-orgcontact-delete-transitivememberof.md)|None|Remove a transitiveMemberOf object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addresses|[physicalOfficeAddress](../resources/microsoft.directoryservices-physicalofficeaddress.md) collection|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|jobTitle|String|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/microsoft.directoryservices-onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|phones|[phone](../resources/microsoft.directoryservices-phone.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directReports|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|manager|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.orgContact",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.orgContact",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "Microsoft.DirectoryServices.physicalOfficeAddress",
      "city": "String",
      "countryOrRegion": "String",
      "officeLocation": "String",
      "postalCode": "String",
      "state": "String",
      "street": "String"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesSyncEnabled": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError",
      "value": "String",
      "category": "String",
      "propertyCausingError": "String",
      "occurredDateTime": "String (timestamp)"
    }
  ],
  "phones": [
    {
      "@odata.type": "Microsoft.DirectoryServices.phone",
      "type": "String",
      "number": "String"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String"
}
```

