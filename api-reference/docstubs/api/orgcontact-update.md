---
title: "Update orgContact"
description: "Update the properties of an orgContact object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update orgContact

Namespace: microsoft.graph

Update the properties of an [orgContact](../resources/orgcontact.md) object.

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
PATCH /contacts/{contactsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [orgContact](../resources/orgcontact.md) object.

The following table shows the properties that are required when you create the [orgContact](../resources/orgcontact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|addresses|[physicalOfficeAddress](../resources/physicalofficeaddress.md) collection|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [orgContact](../resources/orgcontact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/contacts/{contactsId}
Content-Type: application/json
Content-length: 1355

{
  "@odata.type": "#microsoft.graph.orgContact",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:01:31.6341616+03:00"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
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
  "@odata.type": "#microsoft.graph.orgContact",
  "id": "165a8813-8813-165a-1388-5a1613885a16",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:01:31.6341616+03:00"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
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

