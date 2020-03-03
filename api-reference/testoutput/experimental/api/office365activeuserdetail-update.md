---
title: "Update office365ActiveUserDetail"
description: "Update the properties of a office365ActiveUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update office365ActiveUserDetail

Update the properties of a [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.office365ActiveUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [office365ActiveUserDetail](../resources/office365ActiveUserDetail.md) object.

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
If successful, this method returns a `200 OK` response code and an updated [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_office365activeuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.office365ActiveUserDetail not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
  "id": "f706e6a6-e6a6-f706-a6e6-06f7a6e606f7",
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

