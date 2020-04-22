---
title: "Update reviewers"
description: "Update the properties of a reviewers object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update reviewers

Namespace: microsoft.graph

Update the properties of a reviewers object.

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
PATCH /accessReviews/{accessReviewsId}/reviewers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [accessReviewReviewer](../resources/accessreviewreviewer.md) object.

The following table shows the properties that are required when you create the [accessReviewReviewer](../resources/accessreviewreviewer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [accessReviewReviewer](../resources/accessreviewreviewer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_reviewers"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/accessReviews/{accessReviewsId}/reviewers
Content-Type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "displayName": "Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "aedf2ff6-2ff6-aedf-f62f-dfaef62fdfae",
  "displayName": "Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

