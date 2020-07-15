---
title: "List delegatedPermissionClassifications"
description: "Get the delegatedPermissionClassifications from the delegatedPermissionClassifications navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List delegatedPermissionClassifications
Namespace: microsoft.graph

Get the delegatedPermissionClassifications from the delegatedPermissionClassifications navigation property.

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
GET /servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_delegatedpermissionclassification"
}
-->
``` http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedPermissionClassification)"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
      "id": "fc1cedea-edea-fc1c-eaed-1cfceaed1cfc",
      "permissionId": "String",
      "permissionName": "String",
      "classification": "String"
    }
  ]
}
```

