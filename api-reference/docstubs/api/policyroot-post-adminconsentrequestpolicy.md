---
title: "Create adminConsentRequestPolicy"
description: "Create a new adminConsentRequestPolicy object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create adminConsentRequestPolicy

Namespace: microsoft.graph

Create a new adminConsentRequestPolicy object.

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
POST /policies/adminConsentRequestPolicy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.

The following table shows the properties that are required when you create the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|
|notifyReviewers|Boolean|**TODO: Add Description**|
|remindersEnabled|Boolean|**TODO: Add Description**|
|requestDurationInDays|Int32|**TODO: Add Description**|
|reviewers|[accessReviewScope](../resources/accessreviewscope.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_adminconsentrequestpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy
Content-Type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": true,
  "version": 7,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope",
      "query": "Query value",
      "queryType": "Query Type value"
    }
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminconsentrequestpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "id": "5a7b57bf-57bf-5a7b-bf57-7b5abf577b5a",
  "isEnabled": true,
  "version": 7,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope",
      "query": "Query value",
      "queryType": "Query Type value"
    }
  ]
}
```

