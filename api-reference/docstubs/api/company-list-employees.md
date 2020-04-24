---
title: "List employees"
description: "Get the employees from the employees navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List employees

Namespace: microsoft.graph

Get the employees from the employees navigation property.

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
GET /financials/companies/{companyId}/employees
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [employee](../resources/employee.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_employee"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/employees
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.employee)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.employee",
      "id": "9d6aa130-a130-9d6a-30a1-6a9d30a16a9d",
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
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
    }
  ]
}
```

