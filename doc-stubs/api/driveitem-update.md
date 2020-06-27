---
title: "Update driveItem"
description: "Update the properties of a driveItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update driveItem
Namespace: microsoft.graph

Update the properties of a [driveItem](../resources/driveitem.md) object.

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
PATCH /teams/{teamsId}/channels/{channelId}/filesFolder
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [driveItem](../resources/driveitem.md) object.

The following table shows the properties that are required when you create the [driveItem](../resources/driveitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [driveItem](../resources/driveitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_driveitem"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/channels/{channelId}/filesFolder
Content-Type: application/json
Content-length: 51

{
  "@odata.type": "#microsoft.graph.driveItem"
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
  "@odata.type": "#microsoft.graph.driveItem",
  "id": "313cf7d2-f7d2-313c-d2f7-3c31d2f73c31"
}
```

