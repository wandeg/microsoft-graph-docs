---
title: "Update employee"
description: "Update the properties of a employee object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update employee

Namespace: microsoft.graph

Update the properties of a [employee](../resources/employee.md) object.

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
PATCH /financials/companies/{companyId}/employees/{employeeId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [employee](../resources/employee.md) object.

The following table shows the properties that are required when you create the [employee](../resources/employee.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|givenName|String||
|middleName|String||
|surname|String||
|jobTitle|String||
|address|[postalAddressType](../resources/postaladdresstype.md)||
|phoneNumber|String||
|mobilePhone|String||
|email|String||
|personalEmail|String||
|employmentDate|Date||
|terminationDate|Date||
|status|String||
|birthDate|Date||
|statisticsGroupCode|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [employee](../resources/employee.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_employee"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/employees/{employeeId}
Content-type: application/json
Content-length: 838

{
  "@odata.type": "#microsoft.graph.employee",
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
  "statisticsGroupCode": "Statistics Group Code value"
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
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.employee",
  "id": "9a898a90-8a90-9a89-908a-899a908a899a",
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
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00"
}
```

