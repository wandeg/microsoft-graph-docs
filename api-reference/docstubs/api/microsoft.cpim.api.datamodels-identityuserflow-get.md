---
title: "Get identityUserFlow"
description: "Read properties and relationships of an identityUserFlow object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get identityUserFlow

Namespace: microsoft.cpim.api.dataModels

Read properties and relationships of an [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object.

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
GET /identity/userFlows/{identityUserFlowId}
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
If successful, this method returns a `200 OK` response code and an [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/userFlows/{identityUserFlowId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.dataModels.identityUserFlow"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.cpim.api.dataModels.identityUserFlow",
    "id": "68824056-4056-6882-5640-826856408268",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single"
  }
}
```

