---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /education/classes/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [educationClass](../resources/educationclass.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationclass)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "b475b7af-b7af-b475-afb7-75b4afb775b4",
      "displayName": "Display Name value",
      "mailNickname": "Mail Nickname value",
      "description": "Description value",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "Class Code value",
      "externalName": "External Name value",
      "externalId": "External Id value",
      "externalSource": "String",
      "grade": "Grade value",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      },
      "course": {
        "@odata.type": "microsoft.graph.educationCourse"
      }
    }
  ]
}
```

