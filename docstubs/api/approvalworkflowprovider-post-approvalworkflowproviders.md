---
title: "Create approvalWorkflowProvider"
description: "Create a new approvalWorkflowProvider object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create approvalWorkflowProvider

Namespace: microsoft.graph

Create a new [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.

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
POST /approvalWorkflowProviders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object.

The following table shows the properties that are required when you create the [approvalWorkflowProvider](../resources/approvalworkflowprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [approvalWorkflowProvider](../resources/approvalworkflowprovider.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_approvalworkflowprovider_from_approvalworkflowproviders"
}
-->
``` http
POST https://graph.microsoft.com/beta/approvalWorkflowProviders
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
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalworkflowprovider"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 155

{
  "@odata.type": "#microsoft.graph.approvalWorkflowProvider",
  "id": "28dc35c2-35c2-28dc-c235-dc28c235dc28",
  "displayName": "Display Name value"
}
```

