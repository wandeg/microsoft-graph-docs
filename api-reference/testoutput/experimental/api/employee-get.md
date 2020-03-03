---
title: "Get employee"
description: "Read properties and relationships of the employee object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get employee

Namespace: microsoft.graph

Read properties and relationships of the [employee](../resources/employee.md) object.

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
GET /financials/companies/{companyId}/employees/{employeeId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [employee](../resources/employee.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_employee"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/employees/{employeeId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.employee"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1022

{
  "value": {
    "@odata.type": "#microsoft.graph.employee",
    "id": "4afa59a1-59a1-4afa-a159-fa4aa159fa4a",
    "number": "Number value",
    "displayName": "Display Name value",
    "givenName": "Given Name value",
    "middleName": "Middle Name value",
    "surname": "Surname value",
    "jobTitle": "Job Title value",
    "address": {
      "@odata.type": "microsoft.graph.postalAddressType",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryLetterCode": "Country Letter Code value",
      "postalCode": "Postal Code value"
    },
    "phoneNumber": "Phone Number value",
    "mobilePhone": "Mobile Phone value",
    "email": "Email value",
    "personalEmail": "Personal Email value",
    "employmentDate": "Date",
    "terminationDate": "Date",
    "status": "Status value",
    "birthDate": "Date",
    "statisticsGroupCode": "Statistics Group Code value",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
  }
}
```

