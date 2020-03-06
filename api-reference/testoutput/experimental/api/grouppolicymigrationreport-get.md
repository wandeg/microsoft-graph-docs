---
title: "Get groupPolicyMigrationReport"
description: "Read properties and relationships of the groupPolicyMigrationReport object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupPolicyMigrationReport

Namespace: microsoft.graph

Read properties and relationships of the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.

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
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicymigrationreport"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyMigrationReport"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 761

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
    "id": "4139db36-db36-4139-36db-394136db3941",
    "groupPolicyObjectId": "78214cb1-4cb1-7821-b14c-2178b14c2178",
    "displayName": "Display Name value",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
    "groupPolicyCreatedDateTime": "2017-01-01T00:01:36.750057+03:00",
    "groupPolicyLastModifiedDateTime": "2017-01-01T00:03:24.7936609+03:00",
    "migrationReadiness": "String",
    "targetedInActiveDirectory": true,
    "totalSettingsCount": 2,
    "supportedSettingsCount": 6,
    "supportedSettingsPercent": 8
  }
}
```

