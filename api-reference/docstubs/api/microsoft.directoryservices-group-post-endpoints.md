---
title: "Create endpoints"
description: "Create a new endpoints object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create endpoints

Namespace: Microsoft.DirectoryServices

Create a new endpoints object.

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
POST /groups/{groupsId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [endpoint](../resources/microsoft.directoryservices-endpoint.md) object.

The following table shows the properties that are required when you create the [endpoint](../resources/microsoft.directoryservices-endpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|capability|String|**TODO: Add Description**|
|providerId|String|**TODO: Add Description**|
|providerName|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|
|providerResourceId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [endpoint](../resources/microsoft.directoryservices-endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_endpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/groups/{groupsId}/endpoints
Content-Type: application/json
Content-length: 316

{
  "@odata.type": "#Microsoft.DirectoryServices.endpoint",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.endpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.endpoint",
  "id": "f1e186fe-86fe-f1e1-fe86-e1f1fe86e1f1",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
}
```

