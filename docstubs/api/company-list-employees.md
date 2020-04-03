---
title: "List employees"
description: "Get the employees from the employees navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List employees

Namespace: microsoft.graph

Get the employees from the employees navigation property.

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
GET /financials/companies/{companyId}/employees
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [employee](../resources/employee.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_employee"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/employees
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.employee)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.employee",
      "id": "6a5c8f4f-8f4f-6a5c-4f8f-5c6a4f8f5c6a",
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
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
    }
  ]
}
```

