---
title: "List groupPolicyPresentationValueMultiTexts"
description: "List properties and relationships of the groupPolicyPresentationValueMultiText objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicyPresentationValueMultiTexts

List properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) objects.

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
GET ** Collection URI for microsoft.graph.groupPolicyPresentationValueMultiText not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicypresentationvaluemultitext"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.groupPolicyPresentationValueMultiText not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicypresentationvaluemultitext)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
      "id": "109d5cf4-5cf4-109d-f45c-9d10f45c9d10",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
      "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
      "values": [
        "Values value"
      ]
    }
  ]
}
```

