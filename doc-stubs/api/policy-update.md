---
title: "Update policy"
description: "Update the properties of a policy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update policy
Namespace: microsoft.graph

Update the properties of a [policy](../resources/policy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

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
PATCH /legacy/policies/{policyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [policy](../resources/policy.md) object.

The following table shows the properties that are required when you create the [policy](../resources/policy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|alternativeIdentifier|String|**TODO: Add Description**|
|definition|String collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isOrganizationDefault|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [policy](../resources/policy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_policy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/legacy/policies/{policyId}
Content-Type: application/json
Content-length: 354

{
  "@odata.type": "#microsoft.graph.policy",
  "deletedDateTime": "String (timestamp)",
  "alternativeIdentifier": "String",
  "definition": [
    "String"
  ],
  "displayName": "String",
  "isOrganizationDefault": "Boolean",
  "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredential"
    }
  ],
  "type": "String"
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
  "@odata.type": "#microsoft.graph.policy",
  "id": "7e3be4b3-e4b3-7e3b-b3e4-3b7eb3e43b7e",
  "deletedDateTime": "String (timestamp)",
  "alternativeIdentifier": "String",
  "definition": [
    "String"
  ],
  "displayName": "String",
  "isOrganizationDefault": "Boolean",
  "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredential"
    }
  ],
  "type": "String"
}
```

