---
title: "Update userInstallStateSummary"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update userInstallStateSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a userInstallStateSummary object.

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

In the request body, supply JSON representation of the [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a userInstallStateSummary object.

| Property                | Type   | Description                   |
| :---------------------- | :----- | :---------------------------- |
| failedDeviceCount       | Int32  | Failed Device Count.          |
| id                      | String | Key of the entity. Read-only. |
| installedDeviceCount    | Int32  | Installed Device Count.       |
| notInstalledDeviceCount | Int32  | Not installed device count.   |
| userName                | String | User name.                    |

## Response

If successful, this method returns a `200 OK` response code and a userInstallStateSummary object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_userinstallstatesummary"
}
-->

```http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{id}/userStateSummary/{id}

Content-Type: application/json
Content-Length: 198

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "failedDeviceCount": "Int32",
  "installedDeviceCount": "Int32",
  "notInstalledDeviceCount": "Int32",
  "userName": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userInstallStateSummary"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "failedDeviceCount": "Int32",
  "id": "String(identifier)",
  "installedDeviceCount": "Int32",
  "notInstalledDeviceCount": "Int32",
  "userName": "String"
}
}

```