---
title: "Get approvalWorkflowProvider"
description: "Read properties and relationships of the approvalWorkflowProvider object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get approvalWorkflowProvider

Namespace: microsoft.graph

Read properties and relationships of the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.

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
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}
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
If successful, this method returns a `200 OK` response code and [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approvalworkflowprovider"
}
-->
``` http
GET https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalWorkflowProvider"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 180

{
  "value": {
    "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
    "id": "cfedc9c8-c9c8-cfed-c8c9-edcfc8c9edcf",
    "displayName": "Display Name value"
  }
}
```

