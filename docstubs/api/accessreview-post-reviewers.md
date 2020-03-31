---
title: "Add reviewers"
description: "Add reviewers by posting to the reviewers collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add reviewers

Namespace: microsoft.graph

Add reviewers by posting to the reviewers collection.

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
POST /accessReviews/{accessReviewsId}/reviewers/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessReviewReviewer](../resources/accessreviewreviewer.md) object.

The following table shows the properties that are required when you create the [accessReviewReviewer](../resources/accessreviewreviewer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessReviewReviewer](../resources/accessreviewreviewer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accessreviewreviewer_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}/reviewers
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "displayName": "Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessreviewreviewer"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "1685a3ea-a3ea-1685-eaa3-8516eaa38516",
  "displayName": "Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

