---
title: "Update approvalWorkflowProvider"
description: "Update the properties of a approvalWorkflowProvider object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update approvalWorkflowProvider

Namespace: microsoft.graph

Update the properties of a [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.

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
PATCH /approvalWorkflowProviders/{approvalWorkflowProvidersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.

The following table shows the properties that are required when you create the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_approvalworkflowprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}
Content-type: application/json
Content-length: 106

{
  "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
  "id": "cfedc9c8-c9c8-cfed-c8c9-edcfc8c9edcf",
  "displayName": "Display Name value"
}
```

