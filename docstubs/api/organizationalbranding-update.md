---
title: "Update organizationalBranding"
description: "Update the properties of a organizationalBranding object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update organizationalBranding

Namespace: microsoft.graph

Update the properties of a [organizationalBranding](../resources/organizationalbranding.md) object.

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
PATCH /organization/{organizationId}/brandings/{organizationalBrandingId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [organizationalBranding](../resources/organizationalbranding.md) object.

The following table shows the properties that are required when you create the [organizationalBranding](../resources/organizationalbranding.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|backgroundColor|String||
|backgroundImage|Stream||
|bannerLogo|Stream||
|locale|String||
|signInPageText|String||
|squareLogo|Stream||
|usernameHintText|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [organizationalBranding](../resources/organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_organizationalbranding"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/brandings/{organizationalBrandingId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.organizationalBranding",
  "backgroundColor": "Background Color value",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "Locale value",
  "signInPageText": "Sign In Page Text value",
  "squareLogo": "Stream",
  "usernameHintText": "Username Hint Text value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "@odata.type": "#microsoft.graph.organizationalBranding",
  "id": "2a590076-0076-2a59-7600-592a7600592a",
  "backgroundColor": "Background Color value",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "locale": "Locale value",
  "signInPageText": "Sign In Page Text value",
  "squareLogo": "Stream",
  "usernameHintText": "Username Hint Text value"
}
```

