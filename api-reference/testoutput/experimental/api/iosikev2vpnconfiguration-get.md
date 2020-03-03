---
title: "Get iosikEv2VpnConfiguration"
description: "Read properties and relationships of the iosikEv2VpnConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get iosikEv2VpnConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [iosikEv2VpnConfiguration](../resources/iosikev2vpnconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.iosikEv2VpnConfiguration not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [iosikEv2VpnConfiguration](../resources/iosikev2vpnconfiguration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_iosikev2vpnconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.iosikEv2VpnConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.iosikEv2VpnConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4177

{
  "value": {
    "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
    "id": "48f1e8d8-e8d8-48f1-d8e8-f148d8e8f148",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "String"
      ],
      "name": "Name value",
      "ruleType": "String"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "String"
    },
    "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "connectionName": "Connection Name value",
    "connectionType": "String",
    "loginGroupOrDomain": "Login Group Or Domain value",
    "role": "Role value",
    "realm": "Realm value",
    "server": {
      "@odata.type": "microsoft.graph.vpnServer",
      "address": "Address value",
      "isDefaultServer": true
    },
    "identifier": "Identifier value",
    "customData": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ],
    "customKeyValueData": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "enableSplitTunneling": true,
    "authenticationMethod": "String",
    "enablePerApp": true,
    "safariDomains": [
      "Safari Domains value"
    ],
    "onDemandRules": [
      {
        "@odata.type": "microsoft.graph.vpnOnDemandRule",
        "ssids": [
          "Ssids value"
        ],
        "dnsSearchDomains": [
          "Dns Search Domains value"
        ],
        "probeUrl": "https://example.com/probeUrl/",
        "action": "String",
        "domainAction": "String",
        "domains": [
          "Domains value"
        ],
        "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
      }
    ],
    "proxyServer": {
      "@odata.type": "microsoft.graph.vpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "port": 4
    },
    "optInToDeviceIdSharing": true,
    "providerType": "String",
    "userDomain": "User Domain value",
    "strictEnforcement": true,
    "cloudName": "Cloud Name value",
    "excludeList": [
      "Exclude List value"
    ],
    "childSecurityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "String",
      "securityIntegrityAlgorithm": "String",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "clientAuthenticationType": "String",
    "deadPeerDetectionRate": "String",
    "disableMobilityAndMultihoming": true,
    "disableRedirect": true,
    "enableCertificateRevocationCheck": true,
    "enableEAP": true,
    "enablePerfectForwardSecrecy": true,
    "enableUseInternalSubnetAttributes": true,
    "localIdentifier": "String",
    "remoteIdentifier": "Remote Identifier value",
    "securityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
    },
    "serverCertificateCommonName": "Server Certificate Common Name value",
    "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
    "serverCertificateType": "String",
    "sharedSecret": "Shared Secret value",
    "tlsMaximumVersion": "Tls Maximum Version value",
    "tlsMinimumVersion": "Tls Minimum Version value",
    "allowDefaultSecurityAssociationParameters": true,
    "allowDefaultChildSecurityAssociationParameters": true
  }
}
```

