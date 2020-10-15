---
title: "Update deviceInstallState"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update deviceInstallState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a deviceInstallState object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request Body

In the request body, supply JSON representation of the [deviceInstallState](../resources/intune-deviceinstallstate.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a deviceInstallState object.

| Property         | Type           | Description                          |
| :--------------- | :------------- | :----------------------------------- |
| deviceId         | String         | Device Id.                           |
| deviceName       | String         | Device name.                         |
| errorCode        | String         | The error code for install failures. |
| id               | String         | Key of the entity. Read-only.        |
| installState     | String         | The install state of the eBook.      |
| lastSyncDateTime | DateTimeOffset | Last sync date and time.             |
| osDescription    | String         | OS Description.                      |
| osVersion        | String         | OS Version.                          |
| userName         | String         | Device User Name.                    |

## Response

If successful, this method returns a `200 OK` response code and a deviceInstallState object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_deviceinstallstate"
}
-->

```http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{id}/deviceStates/{id}

Content-Type: application/json
Content-Length: 289

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceId": "String",
  "deviceName": "String",
  "errorCode": "String",
  "installState": "String",
  "lastSyncDateTime": "DateTimeOffset",
  "osDescription": "String",
  "osVersion": "String",
  "userName": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.deviceInstallState"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceId": "String",
  "deviceName": "String",
  "errorCode": "String",
  "id": "String(identifier)",
  "installState": "String",
  "lastSyncDateTime": "DateTimeOffset",
  "osDescription": "String",
  "osVersion": "String",
  "userName": "String"
}
}

```