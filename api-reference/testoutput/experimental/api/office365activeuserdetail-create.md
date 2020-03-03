---
title: "Create office365ActiveUserDetail"
description: "Create a new office365ActiveUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365ActiveUserDetail

Namespace: microsoft.graph

Create a new [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.office365ActiveUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.

The following table shows the properties that are required when you create the [office365ActiveUserDetail](../resources/office365activeuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|isDeleted|Boolean||
|deletedDate|Date||
|hasExchangeLicense|Boolean||
|hasOneDriveLicense|Boolean||
|hasSharePointLicense|Boolean||
|hasSkypeForBusinessLicense|Boolean||
|hasYammerLicense|Boolean||
|hasTeamsLicense|Boolean||
|exchangeLastActivityDate|Date||
|oneDriveLastActivityDate|Date||
|sharePointLastActivityDate|Date||
|skypeForBusinessLastActivityDate|Date||
|yammerLastActivityDate|Date||
|teamsLastActivityDate|Date||
|exchangeLicenseAssignDate|Date||
|oneDriveLicenseAssignDate|Date||
|sharePointLicenseAssignDate|Date||
|skypeForBusinessLicenseAssignDate|Date||
|yammerLicenseAssignDate|Date||
|teamsLicenseAssignDate|Date||
|assignedProducts|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365activeuserdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365ActiveUserDetail not found
Content-type: application/json
Content-length: 977

{
  "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
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
    "Assigned Products value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365activeuserdetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
  "id": "188d3c66-3c66-188d-663c-8d18663c8d18",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "displayName": "Display Name value",
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
    "Assigned Products value"
  ]
}
```

