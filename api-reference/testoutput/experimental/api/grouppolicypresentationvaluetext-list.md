---
title: "List groupPolicyPresentationValueTexts"
description: "List properties and relationships of the groupPolicyPresentationValueText objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicyPresentationValueTexts

Namespace: microsoft.graph

List properties and relationships of the [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md) objects.

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
GET ** Collection URI for microsoft.graph.groupPolicyPresentationValueText not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicypresentationvaluetext"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.groupPolicyPresentationValueText not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicypresentationvaluetext)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
      "id": "dcd544bd-44bd-dcd5-bd44-d5dcbd44d5dc",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "value": "Value value"
    }
  ]
}
```

