---
title: "salesNavigatorSaveLeadResource: unsaveVieweeAsLead"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# unsaveVieweeAsLead

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
POST /salesNavigatorSaveLead/unsaveVieweeAsLead
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|viewee|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a Boolean in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "salesnavigatorsaveleadresource_unsavevieweeaslead"
}
-->
``` http
POST https://graph.microsoft.com/beta/salesNavigatorSaveLead/unsaveVieweeAsLead

Content-Type: application/json
Content-length: 26

{
  "viewee": "String"
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
  "value": "Boolean"
}
```

