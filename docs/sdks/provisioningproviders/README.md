# ProvisioningProviders

## Overview

Provisioning Providers

### Available Operations

* [comCrmServiceCommandsSelfServiceResourceGetServiceCommands](#comcrmservicecommandsselfserviceresourcegetservicecommands) - Get Service Commands
* [comCrmServiceCommandsSelfServiceResourceSendServiceCommands](#comcrmservicecommandsselfserviceresourcesendservicecommands) - Send Service Command

## comCrmServiceCommandsSelfServiceResourceGetServiceCommands

Retrieve a list of service commands as implemented in a provisioning adapter. The provisioning adapter’s unique identifier must be specified

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceCommandsSelfServiceResource_getServiceCommands" method="get" path="/self-service/v2/provisioning/service_commands" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.provisioningProviders.comCrmServiceCommandsSelfServiceResourceGetServiceCommands({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { provisioningProvidersComCrmServiceCommandsSelfServiceResourceGetServiceCommands } from "crmcom/funcs/provisioning-providers-com-crm-service-commands-self-service-resource-get-service-commands.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await provisioningProvidersComCrmServiceCommandsSelfServiceResourceGetServiceCommands(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("provisioningProvidersComCrmServiceCommandsSelfServiceResourceGetServiceCommands failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                | Type                                                                                                                                                                                     | Required                                                                                                                                                                                 | Description                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                | [operations.ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsRequest](../../models/operations/com-crm-service-commands-self-service-resource-get-service-commands-request.md)   | :heavy_check_mark:                                                                                                                                                                       | The request object to use for the request.                                                                                                                                               |
| `security`                                                                                                                                                                               | [operations.ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsSecurity](../../models/operations/com-crm-service-commands-self-service-resource-get-service-commands-security.md) | :heavy_check_mark:                                                                                                                                                                       | The security requirements to use for the request.                                                                                                                                        |
| `options`                                                                                                                                                                                | RequestOptions                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                       | Used to set various options for making HTTP requests.                                                                                                                                    |
| `options.fetchOptions`                                                                                                                                                                   | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                  | :heavy_minus_sign:                                                                                                                                                                       | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.           |
| `options.retries`                                                                                                                                                                        | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                       | Enables retrying HTTP requests under certain failure conditions.                                                                                                                         |

### Response

**Promise\<[operations.ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsResponse](../../models/operations/com-crm-service-commands-self-service-resource-get-service-commands-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceCommandsSelfServiceResourceSendServiceCommands

Send an command for a service over to the provisioning adapter. The supported commands as well as detailed information on how to call them such as the required input parameters, can be retrieved from the plugin integration via the GET provisioning/service_commands Web API.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceCommandsSelfServiceResource_sendServiceCommands" method="post" path="/self-service/v2/provisioning/service_commands" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.provisioningProviders.comCrmServiceCommandsSelfServiceResourceSendServiceCommands({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    integrationId: "",
    serviceId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
    code: "RESET_SERVICE",
    contact: {
      id: "",
      name: "John Smith",
      code: "A0111012",
    },
    metadataAttributes: [
      {
        key: "pin",
        value: "1234",
      },
    ],
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { provisioningProvidersComCrmServiceCommandsSelfServiceResourceSendServiceCommands } from "crmcom/funcs/provisioning-providers-com-crm-service-commands-self-service-resource-send-service-commands.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await provisioningProvidersComCrmServiceCommandsSelfServiceResourceSendServiceCommands(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    integrationId: "",
    serviceId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
    code: "RESET_SERVICE",
    contact: {
      id: "",
      name: "John Smith",
      code: "A0111012",
    },
    metadataAttributes: [
      {
        key: "pin",
        value: "1234",
      },
    ],
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("provisioningProvidersComCrmServiceCommandsSelfServiceResourceSendServiceCommands failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                  | Type                                                                                                                                                                                       | Required                                                                                                                                                                                   | Description                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                                  | [operations.ComCrmServiceCommandsSelfServiceResourceSendServiceCommandsRequest](../../models/operations/com-crm-service-commands-self-service-resource-send-service-commands-request.md)   | :heavy_check_mark:                                                                                                                                                                         | The request object to use for the request.                                                                                                                                                 |
| `security`                                                                                                                                                                                 | [operations.ComCrmServiceCommandsSelfServiceResourceSendServiceCommandsSecurity](../../models/operations/com-crm-service-commands-self-service-resource-send-service-commands-security.md) | :heavy_check_mark:                                                                                                                                                                         | The security requirements to use for the request.                                                                                                                                          |
| `options`                                                                                                                                                                                  | RequestOptions                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                         | Used to set various options for making HTTP requests.                                                                                                                                      |
| `options.fetchOptions`                                                                                                                                                                     | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                    | :heavy_minus_sign:                                                                                                                                                                         | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.             |
| `options.retries`                                                                                                                                                                          | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                         | Enables retrying HTTP requests under certain failure conditions.                                                                                                                           |

### Response

**Promise\<[operations.ComCrmServiceCommandsSelfServiceResourceSendServiceCommandsResponse](../../models/operations/com-crm-service-commands-self-service-resource-send-service-commands-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |