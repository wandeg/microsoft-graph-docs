---
title: "Update uploadAgent"
description: "Update the properties of an uploadAgent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update uploadAgent

Namespace: microsoft.graph

Update the properties of an uploadAgent object.

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
PATCH /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/uploadAgent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.

The following table shows the properties that are required when you create the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_uploadagent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/uploadAgent
Content-Type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "description": "Description value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00"
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
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "id": "211b34ad-34ad-211b-ad34-1b21ad341b21",
  "description": "Description value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00"
}
```

