# ApprovalRequests

## Overview

Approval Requests

### Available Operations

* [comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest](#comcrmapprovalrequestselfserviceresourceacceptapprovalrequest) - Approve an Approval Request
* [comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction](#comcrmapprovalrequestselfserviceresourceacceptapprovalrequestaction) - Approve an Approval Request
* [comCrmApprovalRequestSelfServiceResourceRejectApprovalRequest](#comcrmapprovalrequestselfserviceresourcerejectapprovalrequest) - Show the Reject an Approval Request Form
* [comCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction](#comcrmapprovalrequestselfserviceresourcerejectapprovalrequestaction) - Reject an Approval Request
* [comCrmApprovalRequestSelfServiceResourcePerformActions](#comcrmapprovalrequestselfserviceresourceperformactions) - Perform Approval Request Actions
* [comCrmApprovalRequestSelfServiceResourceList](#comcrmapprovalrequestselfserviceresourcelist) - List Approval Requests

## comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest

Accept a pending approval request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApprovalRequestSelfServiceResource_acceptApprovalRequest" method="get" path="/self-service/v2/approval_requests/accept/{token}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.approvalRequests.comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest({
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest } from "crmcom/funcs/approval-requests-com-crm-approval-request-self-service-resource-accept-approval-request.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest(crmcom, {
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                    | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                    | [operations.ComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestRequest](../../models/operations/com-crm-approval-request-self-service-resource-accept-approval-request-request.md) | :heavy_check_mark:                                                                                                                                                                           | The request object to use for the request.                                                                                                                                                   |
| `options`                                                                                                                                                                                    | RequestOptions                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                           | Used to set various options for making HTTP requests.                                                                                                                                        |
| `options.fetchOptions`                                                                                                                                                                       | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                      | :heavy_minus_sign:                                                                                                                                                                           | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.               |
| `options.retries`                                                                                                                                                                            | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                           | Enables retrying HTTP requests under certain failure conditions.                                                                                                                             |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction

Accept a pending approval request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApprovalRequestSelfServiceResource_acceptApprovalRequestAction" method="post" path="/self-service/v2/approval_requests/accept/{token}/action" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.approvalRequests.comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction({
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
    body: {},
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction,
} from "crmcom/funcs/approval-requests-com-crm-approval-request-self-service-resource-accept-approval-request-action.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction(crmcom, {
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                 | Type                                                                                                                                                                                                      | Required                                                                                                                                                                                                  | Description                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                 | [operations.ComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestActionRequest](../../models/operations/com-crm-approval-request-self-service-resource-accept-approval-request-action-request.md) | :heavy_check_mark:                                                                                                                                                                                        | The request object to use for the request.                                                                                                                                                                |
| `options`                                                                                                                                                                                                 | RequestOptions                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                        | Used to set various options for making HTTP requests.                                                                                                                                                     |
| `options.fetchOptions`                                                                                                                                                                                    | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                        | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                            |
| `options.retries`                                                                                                                                                                                         | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                        | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                          |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApprovalRequestSelfServiceResourceRejectApprovalRequest

Reject a pending approval request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApprovalRequestSelfServiceResource_rejectApprovalRequest" method="get" path="/self-service/v2/approval_requests/reject/{token}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.approvalRequests.comCrmApprovalRequestSelfServiceResourceRejectApprovalRequest({
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequest } from "crmcom/funcs/approval-requests-com-crm-approval-request-self-service-resource-reject-approval-request.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequest(crmcom, {
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequest failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                    | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                    | [operations.ComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestRequest](../../models/operations/com-crm-approval-request-self-service-resource-reject-approval-request-request.md) | :heavy_check_mark:                                                                                                                                                                           | The request object to use for the request.                                                                                                                                                   |
| `options`                                                                                                                                                                                    | RequestOptions                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                           | Used to set various options for making HTTP requests.                                                                                                                                        |
| `options.fetchOptions`                                                                                                                                                                       | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                      | :heavy_minus_sign:                                                                                                                                                                           | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.               |
| `options.retries`                                                                                                                                                                            | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                           | Enables retrying HTTP requests under certain failure conditions.                                                                                                                             |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction

Reject a pending approval request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApprovalRequestSelfServiceResource_rejectApprovalRequestAction" method="post" path="/self-service/v2/approval_requests/reject/{token}/action" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.approvalRequests.comCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction({
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
    body: {},
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction,
} from "crmcom/funcs/approval-requests-com-crm-approval-request-self-service-resource-reject-approval-request-action.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction(crmcom, {
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                 | Type                                                                                                                                                                                                      | Required                                                                                                                                                                                                  | Description                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                 | [operations.ComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestActionRequest](../../models/operations/com-crm-approval-request-self-service-resource-reject-approval-request-action-request.md) | :heavy_check_mark:                                                                                                                                                                                        | The request object to use for the request.                                                                                                                                                                |
| `options`                                                                                                                                                                                                 | RequestOptions                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                        | Used to set various options for making HTTP requests.                                                                                                                                                     |
| `options.fetchOptions`                                                                                                                                                                                    | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                        | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                            |
| `options.retries`                                                                                                                                                                                         | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                        | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                          |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApprovalRequestSelfServiceResourcePerformActions

Update an existing approval request

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApprovalRequestSelfServiceResource_performActions" method="post" path="/self-service/v2/approval_requests/{id}/actions" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.approvalRequests.comCrmApprovalRequestSelfServiceResourcePerformActions({
    id: "a6ecbc14-5622-0e30-b629-b1289963f7d2",
    body: {
      action: "REJECT",
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
import { approvalRequestsComCrmApprovalRequestSelfServiceResourcePerformActions } from "crmcom/funcs/approval-requests-com-crm-approval-request-self-service-resource-perform-actions.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await approvalRequestsComCrmApprovalRequestSelfServiceResourcePerformActions(crmcom, {
    id: "a6ecbc14-5622-0e30-b629-b1289963f7d2",
    body: {
      action: "REJECT",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("approvalRequestsComCrmApprovalRequestSelfServiceResourcePerformActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmApprovalRequestSelfServiceResourcePerformActionsRequest](../../models/operations/com-crm-approval-request-self-service-resource-perform-actions-request.md)  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmApprovalRequestSelfServiceResourcePerformActionsResponse](../../models/operations/com-crm-approval-request-self-service-resource-perform-actions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApprovalRequestSelfServiceResourceList

Retrieve all approval requests for a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApprovalRequestSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/approval_requests" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.approvalRequests.comCrmApprovalRequestSelfServiceResourceList({
    id: "b2157d75-7959-83dc-fdfa-cacba764d4d4",
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { approvalRequestsComCrmApprovalRequestSelfServiceResourceList } from "crmcom/funcs/approval-requests-com-crm-approval-request-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await approvalRequestsComCrmApprovalRequestSelfServiceResourceList(crmcom, {
    id: "b2157d75-7959-83dc-fdfa-cacba764d4d4",
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("approvalRequestsComCrmApprovalRequestSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmApprovalRequestSelfServiceResourceListRequest](../../models/operations/com-crm-approval-request-self-service-resource-list-request.md)                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmApprovalRequestSelfServiceResourceListResponse](../../models/operations/com-crm-approval-request-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |