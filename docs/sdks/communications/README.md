# Communications

## Overview

Communications

### Available Operations

* [crmComCommunicationSelfServiceResourceGetSingle](#crmcomcommunicationselfserviceresourcegetsingle) - Get Communications
* [crmComCommunicationSelfServiceResourceCommunicationActions](#crmcomcommunicationselfserviceresourcecommunicationactions) - Communications Actions
* [crmComCommunicationSelfServiceResourceList](#crmcomcommunicationselfserviceresourcelist) - List Communications
* [crmComPrintoutSelfServiceResourceOutput](#crmcomprintoutselfserviceresourceoutput) - Printout

## crmComCommunicationSelfServiceResourceGetSingle

Get a specific contact’s communication

### Example Usage

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_getSingle" method="get" path="/self-service/v2/communications/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceGetSingle({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceGetSingle } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-get-single.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceGetSingle(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CrmComCommunicationSelfServiceResourceGetSingleRequest](../../models/operations/crm-com-communication-self-service-resource-get-single-request.md)                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CrmComCommunicationSelfServiceResourceGetSingleResponse](../../models/operations/crm-com-communication-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## crmComCommunicationSelfServiceResourceCommunicationActions

Mark an existing communication as viewed and/or archived

### Example Usage

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_communicationActions" method="put" path="/self-service/v2/communications/{id}/actions" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceCommunicationActions({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      viewed: true,
      archived: false,
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceCommunicationActions } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-communication-actions.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceCommunicationActions(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      viewed: true,
      archived: false,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceCommunicationActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                            | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                            | [operations.CrmComCommunicationSelfServiceResourceCommunicationActionsRequest](../../models/operations/crm-com-communication-self-service-resource-communication-actions-request.md) | :heavy_check_mark:                                                                                                                                                                   | The request object to use for the request.                                                                                                                                           |
| `options`                                                                                                                                                                            | RequestOptions                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                   | Used to set various options for making HTTP requests.                                                                                                                                |
| `options.fetchOptions`                                                                                                                                                               | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                              | :heavy_minus_sign:                                                                                                                                                                   | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.       |
| `options.retries`                                                                                                                                                                    | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                   | Enables retrying HTTP requests under certain failure conditions.                                                                                                                     |

### Response

**Promise\<[operations.CrmComCommunicationSelfServiceResourceCommunicationActionsResponse](../../models/operations/crm-com-communication-self-service-resource-communication-actions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## crmComCommunicationSelfServiceResourceList

Get a list of a contact’s communications

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/communications" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
    viewed: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceList } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
    viewed: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/communications" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    viewed: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceList } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    viewed: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/communications" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "NAME",
    viewed: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceList } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "NAME",
    viewed: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: POSTED_DATE

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/communications" example="POSTED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
    viewed: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceList } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
    viewed: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="crm.com.CommunicationSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/communications" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communications.crmComCommunicationSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "UPDATED_DATE",
    viewed: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComCommunicationSelfServiceResourceList } from "crmcom/funcs/communications-crm-com-communication-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComCommunicationSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    archived: true,
    page: 20,
    size: 20,
    sort: "UPDATED_DATE",
    viewed: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communicationsCrmComCommunicationSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CrmComCommunicationSelfServiceResourceListRequest](../../models/operations/crm-com-communication-self-service-resource-list-request.md)                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CrmComCommunicationSelfServiceResourceListResponse](../../models/operations/crm-com-communication-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## crmComPrintoutSelfServiceResourceOutput

Request (and retrieve) a printout for an invoice or order
                                    <h4>Notes</h4>
                                    <div><div><div><strong>PRINTOUT FLOW</strong></div><p>Integrating printout export for Contacts should be based on the following APIs</p>
<ol>
<li>Printout</li>
<li>Get (Printout) File</li>
</ol>
</div>
</div>

### Example Usage

<!-- UsageSnippet language="typescript" operationID="crm.com.PrintoutSelfServiceResource_output" method="post" path="/self-service/v2/printout" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.communications.crmComPrintoutSelfServiceResourceOutput({
    entity: {
      type: "ORDERS",
      id: "1d014e8e-4e13-20e9-3727-071f0cef5cb6",
    },
    format: "EMAIL",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communicationsCrmComPrintoutSelfServiceResourceOutput } from "crmcom/funcs/communications-crm-com-printout-self-service-resource-output.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communicationsCrmComPrintoutSelfServiceResourceOutput(crmcom, {
    entity: {
      type: "ORDERS",
      id: "1d014e8e-4e13-20e9-3727-071f0cef5cb6",
    },
    format: "EMAIL",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("communicationsCrmComPrintoutSelfServiceResourceOutput failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CrmComPrintoutSelfServiceResourceOutputRequest](../../models/operations/crm-com-printout-self-service-resource-output-request.md)                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |