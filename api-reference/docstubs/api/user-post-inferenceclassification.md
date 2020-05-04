---
title: "Create inferenceClassification"
description: "Create a new inferenceClassification object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create inferenceClassification

Namespace: microsoft.graph

Create a new inferenceClassification object.

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
POST /me/inferenceClassification
POST /users/{usersId}/inferenceClassification
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [inferenceClassification](../resources/inferenceclassification.md) object.

The following table shows the properties that are required when you create the [inferenceClassification](../resources/inferenceclassification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and an [inferenceClassification](../resources/inferenceclassification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/inferenceClassification
Content-Type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.inferenceClassification"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceclassification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.inferenceClassification",
  "id": "32471903-1903-3247-0319-473203194732"
}
```

