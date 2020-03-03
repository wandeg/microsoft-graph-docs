---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/schools/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [educationSchool](../resources/educationSchool.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/education/schools/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationschool)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 838

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "41bd57cc-57cc-41bd-cc57-bd41cc57bd41",
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

