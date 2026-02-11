# ServiceRequests

## Overview

Service requests shall be created via the self service platform.

### Available Operations

* [comCrmServiceRequestSelfServiceResourceList](#comcrmservicerequestselfserviceresourcelist) - List Service Requests
* [comCrmServiceRequestSelfServiceResourceCreate](#comcrmservicerequestselfserviceresourcecreate) - Create Service Request
* [comCrmQueueSelfServiceResourceList](#comcrmqueueselfserviceresourcelist) - List Service Request Queues
* [comCrmServiceRequestSelfServiceResourceGetFiles](#comcrmservicerequestselfserviceresourcegetfiles) - List Service Request Attachments
* [comCrmServiceRequestSelfServiceResourceCreateServiceRequestFile](#comcrmservicerequestselfserviceresourcecreateservicerequestfile) - Add Service Request Attachment
* [comCrmServiceRequestSelfServiceResourceRemoveFile](#comcrmservicerequestselfserviceresourceremovefile) - Delete Service Request Attachment
* [comCrmServiceRequestSelfServiceResourceGetNotes](#comcrmservicerequestselfserviceresourcegetnotes) - List Service Request Note
* [comCrmServiceRequestSelfServiceResourceCreateNote](#comcrmservicerequestselfserviceresourcecreatenote) - Create Service Request Note

## comCrmServiceRequestSelfServiceResourceList

Retrieve all details relating to service requests created by or for a specific contact

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/service_requests" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceList({
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceList } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceList(crmcom, {
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/service_requests" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceList({
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceList } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceList(crmcom, {
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/service_requests" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceList({
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceList } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceList(crmcom, {
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/service_requests" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceList({
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceList } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceList(crmcom, {
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/service_requests" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceList({
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceList } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceList(crmcom, {
    id: "<id>",
    queueId: "bf58e2a0-f73b-4ebb-8425-92ff4253d6be",
    searchValue: "SR0001ABC",
    states: "NEW",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmServiceRequestSelfServiceResourceListRequest](../../models/operations/com-crm-service-request-self-service-resource-list-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmServiceRequestSelfServiceResourceListResponse](../../models/operations/com-crm-service-request-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRequestSelfServiceResourceCreate

Create a service request for a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_create" method="post" path="/self-service/v2/contacts/{id}/service_requests" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceCreate({
    id: "<id>",
    body: {
      description: "I have a query about the potholes in Nicosia Main Road",
      queueId: "",
      address: {
        id: "61c943c8-dfeb-4c09-a25c-b054f48bf244",
        other: {
          isPrimary: true,
          addressLine1: "Elia Papakyriakou",
          addressLine2: "7 Tower Stars",
          stateProvinceCounty: "Egkomi",
          townCity: "Nicosia",
          postalCode: "2015",
          countryCode: "CYP",
          lat: 35.157115,
          lon: 33.313719,
          googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
        },
      },
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
import { serviceRequestsComCrmServiceRequestSelfServiceResourceCreate } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-create.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceCreate(crmcom, {
    id: "<id>",
    body: {
      description: "I have a query about the potholes in Nicosia Main Road",
      queueId: "",
      address: {
        id: "61c943c8-dfeb-4c09-a25c-b054f48bf244",
        other: {
          isPrimary: true,
          addressLine1: "Elia Papakyriakou",
          addressLine2: "7 Tower Stars",
          stateProvinceCounty: "Egkomi",
          townCity: "Nicosia",
          postalCode: "2015",
          countryCode: "CYP",
          lat: 35.157115,
          lon: 33.313719,
          googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
        },
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceCreate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmServiceRequestSelfServiceResourceCreateRequest](../../models/operations/com-crm-service-request-self-service-resource-create-request.md)                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmServiceRequestSelfServiceResourceCreateResponse](../../models/operations/com-crm-service-request-self-service-resource-create-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmQueueSelfServiceResourceList

Retreieves the configuration of queue settings for service requests

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.QueueSelfServiceResource_list" method="get" path="/self-service/v2/queues" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmQueueSelfServiceResourceList();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmQueueSelfServiceResourceList } from "crmcom/funcs/service-requests-com-crm-queue-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmQueueSelfServiceResourceList(crmcom);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmQueueSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmQueueSelfServiceResourceListRequest](../../models/operations/com-crm-queue-self-service-resource-list-request.md)                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmQueueSelfServiceResourceListResponse](../../models/operations/com-crm-queue-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRequestSelfServiceResourceGetFiles

Retrieve all attachments for a specific service request

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getFiles" method="get" path="/self-service/v2/service_requests/{id}/attachments" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetFiles({
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-files.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles(crmcom, {
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getFiles" method="get" path="/self-service/v2/service_requests/{id}/attachments" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetFiles({
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-files.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles(crmcom, {
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getFiles" method="get" path="/self-service/v2/service_requests/{id}/attachments" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetFiles({
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-files.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles(crmcom, {
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getFiles" method="get" path="/self-service/v2/service_requests/{id}/attachments" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetFiles({
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-files.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles(crmcom, {
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getFiles" method="get" path="/self-service/v2/service_requests/{id}/attachments" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetFiles({
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-files.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles(crmcom, {
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmServiceRequestSelfServiceResourceGetFilesRequest](../../models/operations/com-crm-service-request-self-service-resource-get-files-request.md)                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmServiceRequestSelfServiceResourceGetFilesResponse](../../models/operations/com-crm-service-request-self-service-resource-get-files-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRequestSelfServiceResourceCreateServiceRequestFile

Add an attachment (file or link) to an existing service request. Adding a file attachment is achieved firstly by creating a signature for the file that will be uploaded and then connecting it to the related service request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_createServiceRequestFile" method="post" path="/self-service/v2/service_requests/{id}/attachments" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceCreateServiceRequestFile({
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    body: {
      fileId: "30526723-24a3-e4e3-1a75-b26b1b41f05c",
      link: "https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
      description: "Image 1",
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
import { serviceRequestsComCrmServiceRequestSelfServiceResourceCreateServiceRequestFile } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-create-service-request-file.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceCreateServiceRequestFile(crmcom, {
    id: "6b888b83-b418-752f-604d-0653cf65885d",
    body: {
      fileId: "30526723-24a3-e4e3-1a75-b26b1b41f05c",
      link: "https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
      description: "Image 1",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceCreateServiceRequestFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                         | Type                                                                                                                                                                                              | Required                                                                                                                                                                                          | Description                                                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                         | [operations.ComCrmServiceRequestSelfServiceResourceCreateServiceRequestFileRequest](../../models/operations/com-crm-service-request-self-service-resource-create-service-request-file-request.md) | :heavy_check_mark:                                                                                                                                                                                | The request object to use for the request.                                                                                                                                                        |
| `options`                                                                                                                                                                                         | RequestOptions                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                | Used to set various options for making HTTP requests.                                                                                                                                             |
| `options.fetchOptions`                                                                                                                                                                            | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                    |
| `options.retries`                                                                                                                                                                                 | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                  |

### Response

**Promise\<[operations.ComCrmServiceRequestSelfServiceResourceCreateServiceRequestFileResponse](../../models/operations/com-crm-service-request-self-service-resource-create-service-request-file-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRequestSelfServiceResourceRemoveFile

Delete an attachment file for a service request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_removeFile" method="delete" path="/self-service/v2/service_requests/{id}/attachments/{attachment_id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceRemoveFile({
    attachmentId: "8dfc2223-edca-f05d-820b-dc96ba9df2c2",
    id: "6b888b83-b418-752f-604d-0653cf65885d",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceRemoveFile } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-remove-file.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceRemoveFile(crmcom, {
    attachmentId: "8dfc2223-edca-f05d-820b-dc96ba9df2c2",
    id: "6b888b83-b418-752f-604d-0653cf65885d",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceRemoveFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmServiceRequestSelfServiceResourceRemoveFileRequest](../../models/operations/com-crm-service-request-self-service-resource-remove-file-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRequestSelfServiceResourceGetNotes

Retrieve all notes created by the contact for a single service request. Notes created by system users are not included in the response.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getNotes" method="get" path="/self-service/v2/service_requests/{id}/notes" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetNotes({
    id: "<id>",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-notes.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getNotes" method="get" path="/self-service/v2/service_requests/{id}/notes" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetNotes({
    id: "<id>",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-notes.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getNotes" method="get" path="/self-service/v2/service_requests/{id}/notes" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetNotes({
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-notes.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getNotes" method="get" path="/self-service/v2/service_requests/{id}/notes" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetNotes({
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-notes.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_getNotes" method="get" path="/self-service/v2/service_requests/{id}/notes" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceGetNotes({
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-get-notes.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmServiceRequestSelfServiceResourceGetNotesRequest](../../models/operations/com-crm-service-request-self-service-resource-get-notes-request.md)                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmServiceRequestSelfServiceResourceGetNotesResponse](../../models/operations/com-crm-service-request-self-service-resource-get-notes-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRequestSelfServiceResourceCreateNote

Create a note for a service request raised by a contact via a front-end app.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRequestSelfServiceResource_createNote" method="post" path="/self-service/v2/service_requests/{id}/notes" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.serviceRequests.comCrmServiceRequestSelfServiceResourceCreateNote({
    id: "<id>",
    body: {
      note: "After my telephone conversation with Zack this morning, it was decided that....",
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
import { serviceRequestsComCrmServiceRequestSelfServiceResourceCreateNote } from "crmcom/funcs/service-requests-com-crm-service-request-self-service-resource-create-note.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await serviceRequestsComCrmServiceRequestSelfServiceResourceCreateNote(crmcom, {
    id: "<id>",
    body: {
      note: "After my telephone conversation with Zack this morning, it was decided that....",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("serviceRequestsComCrmServiceRequestSelfServiceResourceCreateNote failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmServiceRequestSelfServiceResourceCreateNoteRequest](../../models/operations/com-crm-service-request-self-service-resource-create-note-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmServiceRequestSelfServiceResourceCreateNoteResponse](../../models/operations/com-crm-service-request-self-service-resource-create-note-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |