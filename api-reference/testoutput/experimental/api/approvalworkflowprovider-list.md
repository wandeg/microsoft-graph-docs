---
title: "List approvalWorkflowProviders"
description: "List properties and relationships of the approvalWorkflowProvider objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List approvalWorkflowProviders

Namespace: microsoft.graph

List properties and relationships of the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) objects.

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
GET /approvalWorkflowProviders
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approvalworkflowprovider"
}
-->
``` http
GET https://graph.microsoft.com/localtest/approvalWorkflowProviders
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approvalworkflowprovider)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
      "id": "966bc148-c148-966b-48c1-6b9648c16b96",
      "displayName": "Display Name value"
    }
  ]
}
```

