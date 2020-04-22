---
title: "Add schools"
description: "Add schools by posting to the schools collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Add schools

Namespace: microsoft.graph

Add schools by posting to the schools collection.

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
POST /education/classes/{educationClassId}/schools/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [educationSchool](../resources/educationschool.md) object.

The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|description|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|externalSource|educationExternalSource|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md). Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|externalPrincipalId|String|**TODO: Add Description**|
|lowestGrade|String|**TODO: Add Description**|
|highestGrade|String|**TODO: Add Description**|
|schoolNumber|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|phone|String|**TODO: Add Description**|
|fax|String|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and an [educationSchool](../resources/educationschool.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/schools/$ref
Content-Type: application/json
Content-length: 1104

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "displayName": "Display Name value",
  "description": "Description value",
  "externalSource": "String",
  "principalEmail": "Principal Email value",
  "principalName": "Principal Name value",
  "externalPrincipalId": "External Principal Id value",
  "lowestGrade": "Lowest Grade value",
  "highestGrade": "Highest Grade value",
  "schoolNumber": "School Number value",
  "externalId": "External Id value",
  "phone": "Phone value",
  "fax": "Fax value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationschool"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "3c17d181-d181-3c17-81d1-173c81d1173c",
  "displayName": "Display Name value",
  "description": "Description value",
  "externalSource": "String",
  "principalEmail": "Principal Email value",
  "principalName": "Principal Name value",
  "externalPrincipalId": "External Principal Id value",
  "lowestGrade": "Lowest Grade value",
  "highestGrade": "Highest Grade value",
  "schoolNumber": "School Number value",
  "externalId": "External Id value",
  "phone": "Phone value",
  "fax": "Fax value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  }
}
```

