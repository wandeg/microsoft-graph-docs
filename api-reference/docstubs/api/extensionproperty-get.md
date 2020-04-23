---
title: "Get extensionProperty"
description: "Read the properties and relationships of an extensionProperty object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get extensionProperty

Namespace: microsoft.graph

Read the properties and relationships of an [extensionProperty](../resources/extensionproperty.md) object.

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
GET /applications/{applicationsId}/extensionProperties/{extensionPropertyId}
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
If successful, this method returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_extensionproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/extensionProperties/{extensionPropertyId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.extensionProperty",
    "id": "1dc072ff-72ff-1dc0-ff72-c01dff72c01d",
    "deletedDateTime": "2016-12-31T23:58:36.4652914+03:00",
    "appDisplayName": "App Display Name value",
    "name": "Name value",
    "dataType": "Data Type value",
    "isSyncedFromOnPremises": true,
    "targetObjects": [
      "Target Objects value"
    ]
  }
}
```

