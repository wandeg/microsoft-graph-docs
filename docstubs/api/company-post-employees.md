---
title: "Add employees"
description: "Add employees by posting to the employees collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add employees

Namespace: microsoft.graph

Add employees by posting to the employees collection.

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
POST /financials/companies/{companyId}/employees/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [employee](../resources/employee.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_employee_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/employees
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
  "truncated": true,
  "@odata.type": "microsoft.graph.employee"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.employee",
  "id": "b3d5d176-d176-b3d5-76d1-d5b376d1d5b3",
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
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

