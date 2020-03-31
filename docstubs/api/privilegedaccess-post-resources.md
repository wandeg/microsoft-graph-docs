---
title: "Add resources"
description: "Add resources by posting to the resources collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add resources

Namespace: microsoft.graph

Add resources by posting to the resources collection.

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
POST /privilegedAccess/{privilegedAccessId}/resources/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [governanceResource](../resources/governanceresource.md) object.

The following table shows the properties that are required when you create the [governanceResource](../resources/governanceresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|type|String||
|displayName|String||
|status|String||
|registeredDateTime|DateTimeOffset||
|registeredRoot|String||



## Response
If successful, this method returns a `201 Created` response code and a [governanceResource](../resources/governanceresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_governanceresource_from_governanceresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}/resources
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2016-12-31T23:57:00.7724124+03:00",
  "registeredRoot": "Registered Root value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "id": "1b835a92-5a92-1b83-925a-831b925a831b",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2016-12-31T23:57:00.7724124+03:00",
  "registeredRoot": "Registered Root value"
}
```

