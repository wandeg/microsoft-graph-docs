---
title: "List skills"
description: "Get the skillProficiencies from the skills navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List skills

Namespace: microsoft.graph

Get the skillProficiencies from the skills navigation property.

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
GET /me/profile/skills
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [skillProficiency](../resources/skillproficiency.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_skillproficiency"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/skills
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skillproficiency)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1184

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skillProficiency",
      "id": "77f14a8d-4a8d-77f1-8d4a-f1778d4af177",
      "allowedAudiences": "String",
      "inference": {
        "@odata.type": "microsoft.graph.inferenceData",
        "confidenceScore": "Double",
        "userHasVerifiedAccuracy": true
      },
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "categories": [
        "Categories value"
      ],
      "displayName": "Display Name value",
      "proficiency": "String",
      "webUrl": "https://example.com/webUrl/"
    }
  ]
}
```

