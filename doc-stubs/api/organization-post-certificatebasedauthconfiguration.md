---
title: "Add certificateBasedAuthConfiguration"
description: "Add certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add certificateBasedAuthConfiguration

Namespace: microsoft.graph

Add certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection.

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
POST ** Collection URI for microsoft.graph.certificateBasedAuthConfiguration not found/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

The following table shows the properties that are required when you create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|certificateAuthorities|[certificateAuthority](../resources/certificateauthority.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.certificateBasedAuthConfiguration not found/$ref
Content-Type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
  "certificateAuthorities": [
    {
      "@odata.type": "microsoft.graph.certificateAuthority"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificatebasedauthconfiguration"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
  "id": "468dac06-ac06-468d-06ac-8d4606ac8d46",
  "certificateAuthorities": [
    {
      "@odata.type": "microsoft.graph.certificateAuthority"
    }
  ]
}
```

