---
title: "reportRoot: getOffice365ActiveUserDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getOffice365ActiveUserDetail

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getOffice365ActiveUserDetail
GET /print/reports/{reportRootId}/getOffice365ActiveUserDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response

If successful, this function returns a `200 OK` response code and a [office365ActiveUserDetail](../resources/office365activeuserdetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365activeuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
      "id": "String (identifier)",
      "reportRefreshDate": "Date",
      "userPrincipalName": "String",
      "displayName": "String",
      "isDeleted": "Boolean",
      "deletedDate": "Date",
      "hasExchangeLicense": "Boolean",
      "hasOneDriveLicense": "Boolean",
      "hasSharePointLicense": "Boolean",
      "hasSkypeForBusinessLicense": "Boolean",
      "hasYammerLicense": "Boolean",
      "hasTeamsLicense": "Boolean",
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
  ]
}
```

