﻿# Get directoryObject

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Read properties and relationships of the [directoryObject](../resources/intune_mam_directoryobject.md) object.
## Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementApps.ReadWrite.All; DeviceManagementApps.Read.All*
## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /managedAppPolicies/{managedAppPoliciesId}/targetedSecurityGroups/{directoryObjectId}
GET /managedAppPolicies/{managedAppPoliciesId}/microsoft.graph.targetedManagedAppProtection/targetedSecurityGroups/{directoryObjectId}
GET /managedAppPolicies/{managedAppPoliciesId}/microsoft.graph.targetedManagedAppConfiguration/targetedSecurityGroups/{directoryObjectId}
```

## Optional query parameters
This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.
## Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [directoryObject](../resources/intune_mam_directoryobject.md) object in the response body.

## Example
### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/managedAppPolicies/{managedAppPoliciesId}/targetedSecurityGroups/{directoryObjectId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 129

{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "67d4444d-444d-67d4-4d44-d4674d44d467"
  }
}
```



