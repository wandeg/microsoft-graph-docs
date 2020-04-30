---
title: "Create orgContact"
description: "Create a new orgContact object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create orgContact

Namespace: Microsoft.DirectoryServices

Create a new [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object.

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
POST /contacts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object.

The following table shows the properties that are required when you create the [orgContact](../resources/microsoft.directoryservices-orgcontact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|addresses|[physicalOfficeAddress](../resources/microsoft.directoryservices-physicalofficeaddress.md) collection|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/microsoft.directoryservices-onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|phones|[phone](../resources/microsoft.directoryservices-phone.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_orgcontact_from_contacts"
}
-->
``` http
POST https://graph.microsoft.com/changelog/contacts
Content-Type: application/json
Content-length: 1403

{
  "@odata.type": "#Microsoft.DirectoryServices.orgContact",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "addresses": [
    {
      "@odata.type": "Microsoft.DirectoryServices.physicalOfficeAddress",
      "city": "City value",
      "countryOrRegion": "Country Or Region value",
      "officeLocation": "Office Location value",
      "postalCode": "Postal Code value",
      "state": "State value",
      "street": "Street value"
    }
  ],
  "companyName": "Company Name value",
  "department": "Department value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "jobTitle": "Job Title value",
  "mail": "Mail value",
  "mailNickname": "Mail Nickname value",
  "onPremisesSyncEnabled": true,
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:32.7107544+00:00"
    }
  ],
  "phones": [
    {
      "@odata.type": "Microsoft.DirectoryServices.phone",
      "type": "String",
      "number": "Number value"
    }
  ],
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "surname": "Surname value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.orgcontact"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.orgContact",
  "id": "d45be9bb-e9bb-d45b-bbe9-5bd4bbe95bd4",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "addresses": [
    {
      "@odata.type": "Microsoft.DirectoryServices.physicalOfficeAddress",
      "city": "City value",
      "countryOrRegion": "Country Or Region value",
      "officeLocation": "Office Location value",
      "postalCode": "Postal Code value",
      "state": "State value",
      "street": "Street value"
    }
  ],
  "companyName": "Company Name value",
  "department": "Department value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "jobTitle": "Job Title value",
  "mail": "Mail value",
  "mailNickname": "Mail Nickname value",
  "onPremisesSyncEnabled": true,
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:32.7107544+00:00"
    }
  ],
  "phones": [
    {
      "@odata.type": "Microsoft.DirectoryServices.phone",
      "type": "String",
      "number": "Number value"
    }
  ],
  "proxyAddresses": [
    "Proxy Addresses value"
  ],
  "surname": "Surname value"
}
```

