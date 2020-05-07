---
title: "Create employees"
description: "Create a new employees object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create employees

Namespace: microsoft.graph

Create a new employees object.

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
POST /financials/companies/{companyId}/employees
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and an [employee](../resources/employee.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_employee_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/employees
Content-Type: application/json
Content-length: 531

{
  "@odata.type": "#microsoft.graph.employee",
  "number": "String",
  "displayName": "String",
  "givenName": "String",
  "middleName": "String",
  "surname": "String",
  "jobTitle": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "mobilePhone": "String",
  "email": "String",
  "personalEmail": "String",
  "employmentDate": "Date",
  "terminationDate": "Date",
  "status": "String",
  "birthDate": "Date",
  "statisticsGroupCode": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.employee"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.employee",
  "id": "05af9a78-9a78-05af-789a-af05789aaf05",
  "number": "String",
  "displayName": "String",
  "givenName": "String",
  "middleName": "String",
  "surname": "String",
  "jobTitle": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "mobilePhone": "String",
  "email": "String",
  "personalEmail": "String",
  "employmentDate": "Date",
  "terminationDate": "Date",
  "status": "String",
  "birthDate": "Date",
  "statisticsGroupCode": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

