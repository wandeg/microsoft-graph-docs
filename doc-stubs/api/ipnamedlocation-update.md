---
title: "Update ipNamedLocation"
description: "Update the properties of an ipNamedLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update ipNamedLocation
Namespace: microsoft.graph

Update the properties of an [ipNamedLocation](../resources/ipnamedlocation.md) object.

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
PATCH /ipNamedLocation
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [ipNamedLocation](../resources/ipnamedlocation.md) object.

The following table shows the properties that are required when you create the [ipNamedLocation](../resources/ipnamedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|ipRanges|[ipRange](../resources/intune-iprange.md) collection|**TODO: Add Description**|
|isTrusted|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/ipNamedLocation
Content-Type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.ipNamedLocation",
  "displayName": "String",
  "ipRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange"
    }
  ],
  "isTrusted": "Boolean"
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
  "@odata.type": "#microsoft.graph.ipNamedLocation",
  "id": "a9de9723-9723-a9de-2397-dea92397dea9",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "ipRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange"
    }
  ],
  "isTrusted": "Boolean"
}
```

