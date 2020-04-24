---
title: "Update employee"
description: "Update the properties of an employee object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update employee

Namespace: microsoft.graph

Update the properties of an [employee](../resources/employee.md) object.

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
PATCH /financials/companies/{companyId}/employees/{employeeId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [employee](../resources/employee.md) object.

The following table shows the properties that are required when you create the [employee](../resources/employee.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|middleName|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|personalEmail|String|**TODO: Add Description**|
|employmentDate|Date|**TODO: Add Description**|
|terminationDate|Date|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|birthDate|Date|**TODO: Add Description**|
|statisticsGroupCode|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [employee](../resources/employee.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_employee"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/employees/{employeeId}
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

