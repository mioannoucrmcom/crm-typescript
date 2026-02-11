# Subscriptions

## Overview

Subscriptions

### Available Operations

* [comCrmSubscriptionSelfServiceResourceListSubscriptionServices](#comcrmsubscriptionselfserviceresourcelistsubscriptionservices) - List Contact Services
* [comCrmSubscriptionSelfServiceResourceAddService](#comcrmsubscriptionselfserviceresourceaddservice) - Add Service
* [comCrmSubscriptionSelfServiceResourceListContactSubscriptions](#comcrmsubscriptionselfserviceresourcelistcontactsubscriptions) - List Contact Subscriptions
* [comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions](#comcrmsubscriptionselfserviceresourcelistcontactsubscriptionactions) - List Contact Subscription Actions
* [comCrmEstimateSubscriptionSelfServiceResourceEstimateBilling](#comcrmestimatesubscriptionselfserviceresourceestimatebilling) - Billing
* [comCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription](#comcrmestimatesubscriptionselfserviceresourceestimatesubscription) - Service Delivery
* [comCrmSubscriptionSelfServiceResourceChangeService](#comcrmsubscriptionselfserviceresourcechangeservice) - Update Service
* [comCrmSubscriptionSelfServiceResourceListServiceDevices](#comcrmsubscriptionselfserviceresourcelistservicedevices) - Get Service Devices
* [comCrmSubscriptionSelfServiceResourceListSubscriptionActions](#comcrmsubscriptionselfserviceresourcelistsubscriptionactions) - List Subscription Actions
* [comCrmSubscriptionSelfServiceResourceGetSubscriptionAction](#comcrmsubscriptionselfserviceresourcegetsubscriptionaction) - Get Subscription Action
* [comCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction](#comcrmsubscriptionselfserviceresourceupdatesubscriptionaction) - Update Subscription Action
* [comCrmSubscriptionSelfServiceResourceChange](#comcrmsubscriptionselfserviceresourcechange) - Update Subscription

## comCrmSubscriptionSelfServiceResourceListSubscriptionServices

Returns a list of services to which the contact is subscribed to

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionServices" method="get" path="/self-service/v2/contacts/{id}/services" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionServices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-services.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionServices" method="get" path="/self-service/v2/contacts/{id}/services" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionServices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-services.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionServices" method="get" path="/self-service/v2/contacts/{id}/services" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionServices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-services.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionServices" method="get" path="/self-service/v2/contacts/{id}/services" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionServices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-services.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionServices" method="get" path="/self-service/v2/contacts/{id}/services" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionServices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-services.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                     | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesRequest](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-request.md)   | :heavy_check_mark:                                                                                                                                                                            | The request object to use for the request.                                                                                                                                                    |
| `security`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSecurity](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-security.md) | :heavy_check_mark:                                                                                                                                                                            | The security requirements to use for the request.                                                                                                                                             |
| `options`                                                                                                                                                                                     | RequestOptions                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                            | Used to set various options for making HTTP requests.                                                                                                                                         |
| `options.fetchOptions`                                                                                                                                                                        | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                       | :heavy_minus_sign:                                                                                                                                                                            | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                |
| `options.retries`                                                                                                                                                                             | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                            | Enables retrying HTTP requests under certain failure conditions.                                                                                                                              |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesResponse](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceAddService

Subscribes the customer to new subscription services. A single service can be added per Web API call. In cases where the contact does not own a subscription in the same billing cycle as the new service's cycle, then a new subscirption is also created with this Web API call. Otherwise, the existing subscription is amended with the new service, and this new service's billing cycle is adjusted to the subscription's.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_addService" method="post" path="/self-service/v2/contacts/{id}/services" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceAddService({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      scheduledDate: 1,
      pass: {
        code: "TB68937255",
        pin: "",
      },
      services: [
        {
          productId: "",
          priceTermsId: "",
          quantity: 1,
          components: [
            {
              productId: "",
              priceTermsId: "",
            },
          ],
        },
      ],
      paymentMethodId: "",
      paymentMethodType: "CRM_WALLET",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceAddService } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-add-service.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceAddService(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      scheduledDate: 1,
      pass: {
        code: "TB68937255",
        pin: "",
      },
      services: [
        {
          productId: "",
          priceTermsId: "",
          quantity: 1,
          components: [
            {
              productId: "",
              priceTermsId: "",
            },
          ],
        },
      ],
      paymentMethodId: "",
      paymentMethodType: "CRM_WALLET",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceAddService failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmSubscriptionSelfServiceResourceAddServiceRequest](../../models/operations/com-crm-subscription-self-service-resource-add-service-request.md)                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceAddServiceSecurity](../../models/operations/com-crm-subscription-self-service-resource-add-service-security.md)               | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceAddServiceResponse[]](../../models/.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceListContactSubscriptions

Returns a list of subscriptions owned by a specified contact

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptions" method="get" path="/self-service/v2/contacts/{id}/subscriptions" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscriptions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptions" method="get" path="/self-service/v2/contacts/{id}/subscriptions" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscriptions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptions" method="get" path="/self-service/v2/contacts/{id}/subscriptions" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscriptions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptions" method="get" path="/self-service/v2/contacts/{id}/subscriptions" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscriptions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptions" method="get" path="/self-service/v2/contacts/{id}/subscriptions" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscriptions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                     | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsRequest](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-request.md)   | :heavy_check_mark:                                                                                                                                                                            | The request object to use for the request.                                                                                                                                                    |
| `security`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsSecurity](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-security.md) | :heavy_check_mark:                                                                                                                                                                            | The security requirements to use for the request.                                                                                                                                             |
| `options`                                                                                                                                                                                     | RequestOptions                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                            | Used to set various options for making HTTP requests.                                                                                                                                         |
| `options.fetchOptions`                                                                                                                                                                        | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                       | :heavy_minus_sign:                                                                                                                                                                            | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                |
| `options.retries`                                                                                                                                                                             | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                            | Enables retrying HTTP requests under certain failure conditions.                                                                                                                              |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsResponse](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions

Returns a list of subscription actions of a specified contact (and among all of the cotnact's subscriptions).The list includes actions in any state i.e. Executed, Scheduled, Cancelled and Rejected.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptionActions" method="get" path="/self-service/v2/contacts/{id}/subscriptions/actions" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptionActions" method="get" path="/self-service/v2/contacts/{id}/subscriptions/actions" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptionActions" method="get" path="/self-service/v2/contacts/{id}/subscriptions/actions" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptionActions" method="get" path="/self-service/v2/contacts/{id}/subscriptions/actions" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listContactSubscriptionActions" method="get" path="/self-service/v2/contacts/{id}/subscriptions/actions" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-contact-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    cancelledOnGt: 1618395497,
    cancelledOnGte: 1618395497,
    cancelledOnLt: 1618395497,
    cancelledOnLte: 1618395497,
    scheduledOnGt: 1618395497,
    scheduledOnGte: 1618395497,
    scheduledOnLt: 1618395497,
    scheduledOnLte: 1618395497,
    state: "SCHEDULED,EXECUTED,REJECTED,CANCELLED",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                  | Type                                                                                                                                                                                                       | Required                                                                                                                                                                                                   | Description                                                                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                  | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionActionsRequest](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscription-actions-request.md)   | :heavy_check_mark:                                                                                                                                                                                         | The request object to use for the request.                                                                                                                                                                 |
| `security`                                                                                                                                                                                                 | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionActionsSecurity](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscription-actions-security.md) | :heavy_check_mark:                                                                                                                                                                                         | The security requirements to use for the request.                                                                                                                                                          |
| `options`                                                                                                                                                                                                  | RequestOptions                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                         | Used to set various options for making HTTP requests.                                                                                                                                                      |
| `options.fetchOptions`                                                                                                                                                                                     | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                         | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                             |
| `options.retries`                                                                                                                                                                                          | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                         | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                           |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionActionsResponse](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscription-actions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmEstimateSubscriptionSelfServiceResourceEstimateBilling

Returns an estimation of a customer’s upcoming billing

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.EstimateSubscriptionSelfServiceResource_estimateBilling" method="post" path="/self-service/v2/estimates/billing" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmEstimateSubscriptionSelfServiceResourceEstimateBilling({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    contactId: "",
    accountId: "",
    asOfDate: 1234567,
    upcomingBillingCycles: 3,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateBilling } from "crm/funcs/subscriptions-com-crm-estimate-subscription-self-service-resource-estimate-billing.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateBilling(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    contactId: "",
    accountId: "",
    asOfDate: 1234567,
    upcomingBillingCycles: 3,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateBilling failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                   | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                   | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateBillingRequest](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-billing-request.md)   | :heavy_check_mark:                                                                                                                                                                          | The request object to use for the request.                                                                                                                                                  |
| `security`                                                                                                                                                                                  | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateBillingSecurity](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-billing-security.md) | :heavy_check_mark:                                                                                                                                                                          | The security requirements to use for the request.                                                                                                                                           |
| `options`                                                                                                                                                                                   | RequestOptions                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                          | Used to set various options for making HTTP requests.                                                                                                                                       |
| `options.fetchOptions`                                                                                                                                                                      | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                     | :heavy_minus_sign:                                                                                                                                                                          | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.              |
| `options.retries`                                                                                                                                                                           | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                          | Enables retrying HTTP requests under certain failure conditions.                                                                                                                            |

### Response

**Promise\<[operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateBillingResponse](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-billing-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription

Returns an estimation of a change perfromed on a subscription service, without making the change. The estimation is based on existing services owned by the customer plus any requested changes.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.EstimateSubscriptionSelfServiceResource_estimateSubscription" method="post" path="/self-service/v2/estimates/service_delivery" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.subscriptions.comCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription({
    action: "CHANGE_TERMS",
    contactId: "",
    accountId: "",
    subscriptionId: "",
    scheduledDate: 12345678,
    subscriptionTermChanges: {
      billingDay: {
        dayOfWeek: "MONDAY",
        dayOfMonth: 1,
      },
      paymentMethodId: "",
      fundingSource: "ACCOUNT",
    },
    componentChanges: {
      id: "",
      toBeAdded: [
        {
          productId: "",
          priceTermsId: "",
        },
      ],
      toBeRemoved: [
        {
          id: "",
        },
      ],
    },
    servicesToAdd: [
      {
        productId: "",
        priceTermsId: "",
        quantity: 1,
        components: [
          {
            productId: "",
            priceTermsId: "",
          },
        ],
      },
    ],
    servicesToRemove: [
      {
        id: "",
      },
    ],
    servicesToChange: [
      {
        fromServiceId: "",
        toServiceProductId: "",
        toPriceTermsId: "",
        components: [
          {
            productId: "",
            priceTermsId: "",
          },
        ],
      },
    ],
    serviceTermChanges: [
      {
        serviceId: "",
        autoRenewalPreference: "OPT_IN",
        contractPreference: "RENEW",
        extendBy: {
          uot: "MONTH",
        },
      },
    ],
    classificationCode: "OPT_IN_RENEWALS",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription } from "crm/funcs/subscriptions-com-crm-estimate-subscription-self-service-resource-estimate-subscription.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription(crm, {
    action: "CHANGE_TERMS",
    contactId: "",
    accountId: "",
    subscriptionId: "",
    scheduledDate: 12345678,
    subscriptionTermChanges: {
      billingDay: {
        dayOfWeek: "MONDAY",
        dayOfMonth: 1,
      },
      paymentMethodId: "",
      fundingSource: "ACCOUNT",
    },
    componentChanges: {
      id: "",
      toBeAdded: [
        {
          productId: "",
          priceTermsId: "",
        },
      ],
      toBeRemoved: [
        {
          id: "",
        },
      ],
    },
    servicesToAdd: [
      {
        productId: "",
        priceTermsId: "",
        quantity: 1,
        components: [
          {
            productId: "",
            priceTermsId: "",
          },
        ],
      },
    ],
    servicesToRemove: [
      {
        id: "",
      },
    ],
    servicesToChange: [
      {
        fromServiceId: "",
        toServiceProductId: "",
        toPriceTermsId: "",
        components: [
          {
            productId: "",
            priceTermsId: "",
          },
        ],
      },
    ],
    serviceTermChanges: [
      {
        serviceId: "",
        autoRenewalPreference: "OPT_IN",
        contractPreference: "RENEW",
        extendBy: {
          uot: "MONTH",
        },
      },
    ],
    classificationCode: "OPT_IN_RENEWALS",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                           | Type                                                                                                                                                                                                | Required                                                                                                                                                                                            | Description                                                                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                           | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionRequest](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-request.md) | :heavy_check_mark:                                                                                                                                                                                  | The request object to use for the request.                                                                                                                                                          |
| `options`                                                                                                                                                                                           | RequestOptions                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                                  | Used to set various options for making HTTP requests.                                                                                                                                               |
| `options.fetchOptions`                                                                                                                                                                              | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                  | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                      |
| `options.retries`                                                                                                                                                                                   | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                  | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                    |

### Response

**Promise\<[operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionResponse](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceChangeService

Updates a single suscsription service. A service might change due to various reasons and multiple changes can be logged per Web API log:

- Change the service's state
- Change the service with another service
- Change the service's terms
- Change the service's quantity
- Change a flex service's components

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_changeService" method="put" path="/self-service/v2/services/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceChangeService({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      action: "ACTIVATE",
      categoryId: "",
      scheduledDate: 1,
      useProposedDate: true,
      numberOfDays: 1,
      changeToService: {
        productId: "",
        priceTermsId: "",
      },
      components: {
        added: [
          {
            productId: "",
            priceTermsId: "",
          },
        ],
        removed: [
          {
            id: "",
          },
        ],
      },
      pass: {
        code: "TB68937255",
        pin: "",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceChangeService } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-change-service.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceChangeService(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      action: "ACTIVATE",
      categoryId: "",
      scheduledDate: 1,
      useProposedDate: true,
      numberOfDays: 1,
      changeToService: {
        productId: "",
        priceTermsId: "",
      },
      components: {
        added: [
          {
            productId: "",
            priceTermsId: "",
          },
        ],
        removed: [
          {
            id: "",
          },
        ],
      },
      pass: {
        code: "TB68937255",
        pin: "",
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceChangeService failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmSubscriptionSelfServiceResourceChangeServiceRequest](../../models/operations/com-crm-subscription-self-service-resource-change-service-request.md)           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceChangeServiceSecurity](../../models/operations/com-crm-subscription-self-service-resource-change-service-security.md)         | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceChangeServiceResponse](../../models/operations/com-crm-subscription-self-service-resource-change-service-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceListServiceDevices

Returns a list of Devices to which a service is already enabled on and devices onwed by the contact that are eligible to deliver the specified service

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listServiceDevices" method="get" path="/self-service/v2/services/{id}/devices" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListServiceDevices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
    includeTotal: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-service-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
    includeTotal: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listServiceDevices" method="get" path="/self-service/v2/services/{id}/devices" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListServiceDevices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    includeTotal: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-service-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    includeTotal: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listServiceDevices" method="get" path="/self-service/v2/services/{id}/devices" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListServiceDevices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "NAME",
    includeTotal: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-service-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "NAME",
    includeTotal: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices failed:", res.error);
  }
}

run();
```
### Example Usage: POSTED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listServiceDevices" method="get" path="/self-service/v2/services/{id}/devices" example="POSTED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListServiceDevices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
    includeTotal: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-service-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
    includeTotal: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listServiceDevices" method="get" path="/self-service/v2/services/{id}/devices" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListServiceDevices({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "UPDATED_DATE",
    includeTotal: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-service-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    page: 20,
    size: 20,
    sort: "UPDATED_DATE",
    includeTotal: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                         | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                         | [operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesRequest](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-request.md)   | :heavy_check_mark:                                                                                                                                                                | The request object to use for the request.                                                                                                                                        |
| `security`                                                                                                                                                                        | [operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesSecurity](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-security.md) | :heavy_check_mark:                                                                                                                                                                | The security requirements to use for the request.                                                                                                                                 |
| `options`                                                                                                                                                                         | RequestOptions                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                | Used to set various options for making HTTP requests.                                                                                                                             |
| `options.fetchOptions`                                                                                                                                                            | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                           | :heavy_minus_sign:                                                                                                                                                                | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.    |
| `options.retries`                                                                                                                                                                 | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                | Enables retrying HTTP requests under certain failure conditions.                                                                                                                  |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesResponse](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceListSubscriptionActions

Retrieves a list of actions submitted for a subscription. This set includes all actions already performed on the subscription, actions that failed to be performed as well as actions which are still pending.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionActions" method="get" path="/self-service/v2/subscriptions/actions" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionActions" method="get" path="/self-service/v2/subscriptions/actions" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionActions" method="get" path="/self-service/v2/subscriptions/actions" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionActions" method="get" path="/self-service/v2/subscriptions/actions" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_listSubscriptionActions" method="get" path="/self-service/v2/subscriptions/actions" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceListSubscriptionActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-list-subscription-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    behaviourCode: "ADD_SERVICE",
    businessClassificationCode: "ADD_SERVICE_AS_EFFECTIVE",
    contactId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    isScheduled: true,
    serviceId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    subscriptionId: "9837ee37-a1ab-4a27-9b4b-663c9025a205",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                   | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                   | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsRequest](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-actions-request.md)   | :heavy_check_mark:                                                                                                                                                                          | The request object to use for the request.                                                                                                                                                  |
| `security`                                                                                                                                                                                  | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsSecurity](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-actions-security.md) | :heavy_check_mark:                                                                                                                                                                          | The security requirements to use for the request.                                                                                                                                           |
| `options`                                                                                                                                                                                   | RequestOptions                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                          | Used to set various options for making HTTP requests.                                                                                                                                       |
| `options.fetchOptions`                                                                                                                                                                      | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                     | :heavy_minus_sign:                                                                                                                                                                          | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.              |
| `options.retries`                                                                                                                                                                           | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                          | Enables retrying HTTP requests under certain failure conditions.                                                                                                                            |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsResponse](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-actions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceGetSubscriptionAction

Retrieves detailed information of an existing subscription action

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_getSubscriptionAction" method="get" path="/self-service/v2/subscriptions/actions/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceGetSubscriptionAction({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceGetSubscriptionAction } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-get-subscription-action.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceGetSubscriptionAction(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceGetSubscriptionAction failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                               | Type                                                                                                                                                                                    | Required                                                                                                                                                                                | Description                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                               | [operations.ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionRequest](../../models/operations/com-crm-subscription-self-service-resource-get-subscription-action-request.md)   | :heavy_check_mark:                                                                                                                                                                      | The request object to use for the request.                                                                                                                                              |
| `security`                                                                                                                                                                              | [operations.ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionSecurity](../../models/operations/com-crm-subscription-self-service-resource-get-subscription-action-security.md) | :heavy_check_mark:                                                                                                                                                                      | The security requirements to use for the request.                                                                                                                                       |
| `options`                                                                                                                                                                               | RequestOptions                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                      | Used to set various options for making HTTP requests.                                                                                                                                   |
| `options.fetchOptions`                                                                                                                                                                  | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                 | :heavy_minus_sign:                                                                                                                                                                      | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.          |
| `options.retries`                                                                                                                                                                       | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                      | Enables retrying HTTP requests under certain failure conditions.                                                                                                                        |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionResponse](../../models/operations/com-crm-subscription-self-service-resource-get-subscription-action-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction

Updates an existing subscripton action.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_updateSubscriptionAction" method="put" path="/self-service/v2/subscriptions/actions/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      action: "UPDATE",
      categoryId: "",
      scheduledDate: 1234567,
      periodSettings: {
        durationInDays: 5,
        endsOn: 1234567,
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
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-update-subscription-action.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      action: "UPDATE",
      categoryId: "",
      scheduledDate: 1234567,
      periodSettings: {
        durationInDays: 5,
        endsOn: 1234567,
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                     | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceUpdateSubscriptionActionRequest](../../models/operations/com-crm-subscription-self-service-resource-update-subscription-action-request.md)   | :heavy_check_mark:                                                                                                                                                                            | The request object to use for the request.                                                                                                                                                    |
| `security`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceUpdateSubscriptionActionSecurity](../../models/operations/com-crm-subscription-self-service-resource-update-subscription-action-security.md) | :heavy_check_mark:                                                                                                                                                                            | The security requirements to use for the request.                                                                                                                                             |
| `options`                                                                                                                                                                                     | RequestOptions                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                            | Used to set various options for making HTTP requests.                                                                                                                                         |
| `options.fetchOptions`                                                                                                                                                                        | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                       | :heavy_minus_sign:                                                                                                                                                                            | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                |
| `options.retries`                                                                                                                                                                             | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                            | Enables retrying HTTP requests under certain failure conditions.                                                                                                                              |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceUpdateSubscriptionActionResponse](../../models/operations/com-crm-subscription-self-service-resource-update-subscription-action-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubscriptionSelfServiceResourceChange

Updates subscripion information related to the customer’s billing terms for a set of services

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SubscriptionSelfServiceResource_change" method="put" path="/self-service/v2/subscriptions/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.subscriptions.comCrmSubscriptionSelfServiceResourceChange({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      action: "CHANGE_PAYMENT_METHOD",
      paymentMethodId: "ac5401c3-b2e6-2d99-171f-276084d97536",
      billingDay: {
        dayOfWeek: "MONDAY",
        dayOfMonth: 15,
      },
      fundingSource: "WALLET",
      scheduledDate: 1,
      useProposedDate: true,
      paymentMethodType: "CRM_WALLET",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { subscriptionsComCrmSubscriptionSelfServiceResourceChange } from "crm/funcs/subscriptions-com-crm-subscription-self-service-resource-change.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await subscriptionsComCrmSubscriptionSelfServiceResourceChange(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      action: "CHANGE_PAYMENT_METHOD",
      paymentMethodId: "ac5401c3-b2e6-2d99-171f-276084d97536",
      billingDay: {
        dayOfWeek: "MONDAY",
        dayOfMonth: 15,
      },
      fundingSource: "WALLET",
      scheduledDate: 1,
      useProposedDate: true,
      paymentMethodType: "CRM_WALLET",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("subscriptionsComCrmSubscriptionSelfServiceResourceChange failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmSubscriptionSelfServiceResourceChangeRequest](../../models/operations/com-crm-subscription-self-service-resource-change-request.md)                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceChangeSecurity](../../models/operations/com-crm-subscription-self-service-resource-change-security.md)                        | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmSubscriptionSelfServiceResourceChangeResponse](../../models/operations/com-crm-subscription-self-service-resource-change-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |