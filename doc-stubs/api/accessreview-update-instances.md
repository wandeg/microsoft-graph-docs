---
title: "Update instances"
description: "Update the properties of an instances object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update instances

Namespace: microsoft.graph

Update the properties of an instances object.

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
PATCH ** Collection URI for microsoft.graph.accessReview not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.

The following table shows the properties that are required when you create the [accessReview](../resources/accessreview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|businessFlowTemplateId|String|**TODO: Add Description**|
|reviewerType|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)|**TODO: Add Description**|
|reviewedEntity|[identity](../resources/identity.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessReview](../resources/accessreview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_instances"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.accessReview not found
Content-Type: application/json
Content-length: 516

{
  "@odata.type": "#microsoft.graph.accessReview",
  "displayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "businessFlowTemplateId": "String",
  "reviewerType": "String",
  "description": "String",
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewSettings"
  },
  "reviewedEntity": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessReview",
  "id": "48a14c80-4c80-48a1-804c-a148804ca148",
  "displayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "businessFlowTemplateId": "String",
  "reviewerType": "String",
  "description": "String",
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewSettings"
  },
  "reviewedEntity": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

