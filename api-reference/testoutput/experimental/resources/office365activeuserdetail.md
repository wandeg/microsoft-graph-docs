---
title: "office365ActiveUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# office365ActiveUserDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365ActiveUserDetails](../api/office365activeuserdetail-list.md)|[office365ActiveUserDetail](../resources/office365ActiveUserDetail.md) collection|List properties and relationships of the [office365ActiveUserDetail](../resources/office365activeuserdetail.md) objects.|
|[Get office365ActiveUserDetail](../api/office365activeuserdetail-get.md)|[office365ActiveUserDetail](../resources/office365ActiveUserDetail.md)|Read properties and relationships of the [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.|
|[Create office365ActiveUserDetail](../api/office365activeuserdetail-create.md)|[office365ActiveUserDetail](../resources/office365ActiveUserDetail.md)|Create a new [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.|
|[Delete office365ActiveUserDetail](../api/office365activeuserdetail-delete.md)|None|Deletes a [office365ActiveUserDetail](../resources/office365activeuserdetail.md).|
|[Update office365ActiveUserDetail](../api/office365activeuserdetail-update.md)|[office365ActiveUserDetail](../resources/office365ActiveUserDetail.md)|Update the properties of a [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedProducts|String collection||
|deletedDate|Date||
|displayName|String||
|exchangeLastActivityDate|Date||
|exchangeLicenseAssignDate|Date||
|hasExchangeLicense|Boolean||
|hasOneDriveLicense|Boolean||
|hasSharePointLicense|Boolean||
|hasSkypeForBusinessLicense|Boolean||
|hasTeamsLicense|Boolean||
|hasYammerLicense|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|oneDriveLastActivityDate|Date||
|oneDriveLicenseAssignDate|Date||
|reportRefreshDate|Date||
|sharePointLastActivityDate|Date||
|sharePointLicenseAssignDate|Date||
|skypeForBusinessLastActivityDate|Date||
|skypeForBusinessLicenseAssignDate|Date||
|teamsLastActivityDate|Date||
|teamsLicenseAssignDate|Date||
|userPrincipalName|String||
|yammerLastActivityDate|Date||
|yammerLicenseAssignDate|Date||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "hasExchangeLicense": true,
  "hasOneDriveLicense": true,
  "hasSharePointLicense": true,
  "hasSkypeForBusinessLicense": true,
  "hasYammerLicense": true,
  "hasTeamsLicense": true,
  "exchangeLastActivityDate": "Date",
  "oneDriveLastActivityDate": "Date",
  "sharePointLastActivityDate": "Date",
  "skypeForBusinessLastActivityDate": "Date",
  "yammerLastActivityDate": "Date",
  "teamsLastActivityDate": "Date",
  "exchangeLicenseAssignDate": "Date",
  "oneDriveLicenseAssignDate": "Date",
  "sharePointLicenseAssignDate": "Date",
  "skypeForBusinessLicenseAssignDate": "Date",
  "yammerLicenseAssignDate": "Date",
  "teamsLicenseAssignDate": "Date",
  "assignedProducts": [
    "String"
  ]
}
```

