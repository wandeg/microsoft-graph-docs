---
title: "List office365ActiveUserDetails"
description: "List properties and relationships of the office365ActiveUserDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List office365ActiveUserDetails

Namespace: microsoft.graph

List properties and relationships of the [office365ActiveUserDetail](../resources/office365activeuserdetail.md) objects.

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
GET ** Collection URI for microsoft.graph.office365ActiveUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [office365ActiveUserDetail](../resources/office365activeuserdetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_office365activeuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365ActiveUserDetail not found
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
  ]
}
```

