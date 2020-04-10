---
title: "Add brandings"
description: "Add brandings by posting to the brandings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add brandings

Namespace: microsoft.graph

Add brandings by posting to the brandings collection.

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
POST /organization/{organizationId}/brandings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [organizationalBranding](../resources/organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_organizationalbranding_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/brandings
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
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalbranding"
}
-->
``` http
HTTP/1.1 201 Created
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

