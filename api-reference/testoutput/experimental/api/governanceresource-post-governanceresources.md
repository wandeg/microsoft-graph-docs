---
title: "Create governanceResource"
description: "Create a new governanceResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create governanceResource

Namespace: microsoft.graph

Create a new [governanceResource](../resources/governanceresource.md) object.

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
POST /governanceResources
POST /privilegedAccess/{privilegedAccessId}/resources
```

## Request headers
|Header|Value|
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
POST https://graph.microsoft.com/localtest/governanceResources
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2016-12-31T23:58:28.4802985+03:00",
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
  "id": "bfbf2df6-2df6-bfbf-f62d-bfbff62dbfbf",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2016-12-31T23:58:28.4802985+03:00",
  "registeredRoot": "Registered Root value"
}
```

