---
title: "List approvalWorkflowProviders"
description: "Get a list of the approvalWorkflowProvider objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List approvalWorkflowProviders

Namespace: microsoft.graph

Get a list of the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) objects and their properties.

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
GET /approvalWorkflowProviders
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_approvalworkflowprovider"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/approvalWorkflowProviders
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approvalworkflowprovider)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
      "id": "818590bf-90bf-8185-bf90-8581bf908581",
      "displayName": "Display Name value"
    }
  ]
}
```

