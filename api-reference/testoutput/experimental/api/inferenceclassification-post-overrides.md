---
title: "Add overrides"
description: "Add overrides by posting to the overrides collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add overrides

Add overrides by posting to the overrides collection.

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
POST /me/inferenceClassification/overrides/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the inferenceClassificationOverride object.

The following table shows the properties that are required when you create the inferenceClassificationOverride.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|classifyAs|Enumeration|. Possible values are: `focused`, `other`.|
|senderEmailAddress|[emailAddress](../resources/emailAddress.md)||



## Response
If successful, this method returns a `201 Created` response code and a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/inferenceClassification/overrides
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
  "classifyAs": "String",
  "senderEmailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceclassificationoverride"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
  "id": "92d6a0be-a0be-92d6-bea0-d692bea0d692",
  "classifyAs": "String",
  "senderEmailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  }
}
```

