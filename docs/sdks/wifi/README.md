# Wifi

## Overview

Wifi

### Available Operations

* [comCrmSelfServiceWifiAuthorizationResourceAuthorizeContact](#comcrmselfservicewifiauthorizationresourceauthorizecontact) - Contact WiFi Authorization

## comCrmSelfServiceWifiAuthorizationResourceAuthorizeContact

Authorize a contact over to a WiFi platform for usage allowance consumption

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SelfServiceWifiAuthorizationResource_authorizeContact" method="post" path="/self-service/v2/contacts/{id}/wifi/authorize" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  await crmcom.wifi.comCrmSelfServiceWifiAuthorizationResourceAuthorizeContact({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "eab82829-b65e-ee5a-b0f8-33b8ad48e04e",
    body: {
      macAddress: "01-23-45-67-89-AB",
      estimationId: "0ba7de75-8a68-c19a-3d3a-f4708723a1a4",
      siteId: "onwuq8y1",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { wifiComCrmSelfServiceWifiAuthorizationResourceAuthorizeContact } from "crmcom/funcs/wifi-com-crm-self-service-wifi-authorization-resource-authorize-contact.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await wifiComCrmSelfServiceWifiAuthorizationResourceAuthorizeContact(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "eab82829-b65e-ee5a-b0f8-33b8ad48e04e",
    body: {
      macAddress: "01-23-45-67-89-AB",
      estimationId: "0ba7de75-8a68-c19a-3d3a-f4708723a1a4",
      siteId: "onwuq8y1",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("wifiComCrmSelfServiceWifiAuthorizationResourceAuthorizeContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                               | Type                                                                                                                                                                                    | Required                                                                                                                                                                                | Description                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                               | [operations.ComCrmSelfServiceWifiAuthorizationResourceAuthorizeContactRequest](../../models/operations/com-crm-self-service-wifi-authorization-resource-authorize-contact-request.md)   | :heavy_check_mark:                                                                                                                                                                      | The request object to use for the request.                                                                                                                                              |
| `security`                                                                                                                                                                              | [operations.ComCrmSelfServiceWifiAuthorizationResourceAuthorizeContactSecurity](../../models/operations/com-crm-self-service-wifi-authorization-resource-authorize-contact-security.md) | :heavy_check_mark:                                                                                                                                                                      | The security requirements to use for the request.                                                                                                                                       |
| `options`                                                                                                                                                                               | RequestOptions                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                      | Used to set various options for making HTTP requests.                                                                                                                                   |
| `options.fetchOptions`                                                                                                                                                                  | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                 | :heavy_minus_sign:                                                                                                                                                                      | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.          |
| `options.retries`                                                                                                                                                                       | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                      | Enables retrying HTTP requests under certain failure conditions.                                                                                                                        |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |