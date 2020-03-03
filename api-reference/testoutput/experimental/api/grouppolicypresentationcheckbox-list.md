---
title: "List groupPolicyPresentationCheckBoxes"
description: "List properties and relationships of the groupPolicyPresentationCheckBox objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicyPresentationCheckBoxes

Namespace: microsoft.graph

List properties and relationships of the [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) objects.

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
GET ** Collection URI for microsoft.graph.groupPolicyPresentationCheckBox not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationCheckBox](../resources/grouppolicypresentationcheckbox.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicypresentationcheckbox"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.groupPolicyPresentationCheckBox not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicypresentationcheckbox)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
      "id": "7f1ce9d0-e9d0-7f1c-d0e9-1c7fd0e91c7f",
      "label": "Label value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "defaultChecked": true
    }
  ]
}
```

