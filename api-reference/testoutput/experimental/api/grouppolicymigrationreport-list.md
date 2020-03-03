---
title: "List groupPolicyMigrationReports"
description: "List properties and relationships of the groupPolicyMigrationReport objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicyMigrationReports

Namespace: microsoft.graph

List properties and relationships of the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicymigrationreport"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/groupPolicyMigrationReports
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicymigrationreport)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 803

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
      "id": "f08ed319-d319-f08e-19d3-8ef019d38ef0",
      "groupPolicyObjectId": "1713d55d-d55d-1713-5dd5-13175dd51317",
      "displayName": "Display Name value",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "groupPolicyCreatedDateTime": "2017-01-01T00:01:08.1552648+03:00",
      "groupPolicyLastModifiedDateTime": "2017-01-01T00:03:02.9368554+03:00",
      "migrationReadiness": "String",
      "targetedInActiveDirectory": true,
      "totalSettingsCount": 2,
      "supportedSettingsCount": 6,
      "supportedSettingsPercent": 8
    }
  ]
}
```

