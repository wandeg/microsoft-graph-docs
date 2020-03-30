---
title: "getOffice365ActiveUserDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOffice365ActiveUserDetail

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [office365ActiveUserDetail](../resources/office365activeuserdetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365activeuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
      "id": "17f9ffcc-ffcc-17f9-ccff-f917ccfff917",
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
  ]
}
```

