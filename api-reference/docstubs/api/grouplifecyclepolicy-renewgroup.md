---
title: "groupLifecyclePolicy: renewGroup"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# renewGroup

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /groupLifecyclePolicies/renewGroup
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|groupId|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a Boolean in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}
-->
``` http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup

Content-Type: application/json
Content-length: 35

{
  "groupId": "Group Id value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "edm.boolean"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": true
}
```

