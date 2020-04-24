---
title: "educationSchool: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /education/schools/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [educationSchool](../resources/educationschool.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/schools/delta
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationschool)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "5e102a9e-2a9e-5e10-9e2a-105e9e2a105e",
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
        "@odata.type": "microsoft.graph.identitySet"
      },
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress"
      }
    }
  ]
}
```

