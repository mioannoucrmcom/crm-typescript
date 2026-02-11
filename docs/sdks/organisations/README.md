# Organisations

## Overview

Organisations

### Available Operations

* [comCrmBusinessActivitySelfServiceResourceListBusinessActivities](#comcrmbusinessactivityselfserviceresourcelistbusinessactivities) - List Business Activities
* [comCrmLocationSelfServiceResourceList](#comcrmlocationselfserviceresourcelist) - Locations
* [comCrmLocationSelfServiceResourceListTowns](#comcrmlocationselfserviceresourcelisttowns) - Locations
* [comCrmOrganisationSelfServiceResourceGetSingle](#comcrmorganisationselfserviceresourcegetsingle) - Get Organisation
* [comCrmOrganisationSelfServiceResourceList](#comcrmorganisationselfserviceresourcelist) - Search Organisations
* [comCrmOrganisationSelfServiceResourceSwitchOrganisation](#comcrmorganisationselfserviceresourceswitchorganisation) - Switch Organisations
* [comCrmMerchantSelfServiceResourceList](#comcrmmerchantselfserviceresourcelist) - Participating Merchants

## comCrmBusinessActivitySelfServiceResourceListBusinessActivities

Returns a list of business activities

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.BusinessActivitySelfServiceResource_listBusinessActivities" method="get" path="/self-service/v2/business_activities" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmBusinessActivitySelfServiceResourceListBusinessActivities({
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { organisationsComCrmBusinessActivitySelfServiceResourceListBusinessActivities } from "crm/funcs/organisations-com-crm-business-activity-self-service-resource-list-business-activities.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmBusinessActivitySelfServiceResourceListBusinessActivities(crm, {
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmBusinessActivitySelfServiceResourceListBusinessActivities failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                        | Type                                                                                                                                                                                             | Required                                                                                                                                                                                         | Description                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                                        | [operations.ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesRequest](../../models/operations/com-crm-business-activity-self-service-resource-list-business-activities-request.md) | :heavy_check_mark:                                                                                                                                                                               | The request object to use for the request.                                                                                                                                                       |
| `options`                                                                                                                                                                                        | RequestOptions                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                               | Used to set various options for making HTTP requests.                                                                                                                                            |
| `options.fetchOptions`                                                                                                                                                                           | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                          | :heavy_minus_sign:                                                                                                                                                                               | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                   |
| `options.retries`                                                                                                                                                                                | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                               | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                 |

### Response

**Promise\<[operations.ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesResponse](../../models/operations/com-crm-business-activity-self-service-resource-list-business-activities-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmLocationSelfServiceResourceList

Get a list of organisations (merchants, venues) ordered by nearest first

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.LocationSelfServiceResource_list" method="get" path="/self-service/v2/locations" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmLocationSelfServiceResourceList({
    includeCustomFields: true,
    isOpen: "true",
    lat: "38.91",
    lon: "38.91",
    name: "CRM",
    organisationId: "a3f1f6b3-8d49-3a72-e48e-617dd6004d41",
    within: "154",
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
import { organisationsComCrmLocationSelfServiceResourceList } from "crm/funcs/organisations-com-crm-location-self-service-resource-list.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmLocationSelfServiceResourceList(crm, {
    includeCustomFields: true,
    isOpen: "true",
    lat: "38.91",
    lon: "38.91",
    name: "CRM",
    organisationId: "a3f1f6b3-8d49-3a72-e48e-617dd6004d41",
    within: "154",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmLocationSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmLocationSelfServiceResourceListRequest](../../models/operations/com-crm-location-self-service-resource-list-request.md)                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmLocationSelfServiceResourceListResponse](../../models/operations/com-crm-location-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmLocationSelfServiceResourceListTowns

Get a list of organisations (merchants, venues) ordered by nearest first

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.LocationSelfServiceResource_listTowns" method="get" path="/self-service/v2/locations/towns" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmLocationSelfServiceResourceListTowns();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { organisationsComCrmLocationSelfServiceResourceListTowns } from "crm/funcs/organisations-com-crm-location-self-service-resource-list-towns.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmLocationSelfServiceResourceListTowns(crm);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmLocationSelfServiceResourceListTowns failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmLocationSelfServiceResourceListTownsResponse](../../models/operations/com-crm-location-self-service-resource-list-towns-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrganisationSelfServiceResourceGetSingle

Retrieve all details for a specific organisation

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrganisationSelfServiceResource_getSingle" method="get" path="/self-service/v2/organisations/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmOrganisationSelfServiceResourceGetSingle({
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
import { organisationsComCrmOrganisationSelfServiceResourceGetSingle } from "crm/funcs/organisations-com-crm-organisation-self-service-resource-get-single.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmOrganisationSelfServiceResourceGetSingle(crm, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmOrganisationSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrganisationSelfServiceResourceGetSingleRequest](../../models/operations/com-crm-organisation-self-service-resource-get-single-request.md)                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrganisationSelfServiceResourceGetSingleResponse](../../models/operations/com-crm-organisation-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrganisationSelfServiceResourceList

Retrieve a list of organisations that comprise the business network

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrganisationSelfServiceResource_list" method="get" path="/self-service/v2/organisations/{id}/network" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmOrganisationSelfServiceResourceList({
    id: "<id>",
    customFields: "key;value;key;value",
    distance: 5,
    lat: "\"35.1730837\"",
    lon: "\"33.3761312\"",
    name: "Bravo Coffee",
    tapCode: "01-23-45-67-89-AB",
    type: "MERCHANT",
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
import { organisationsComCrmOrganisationSelfServiceResourceList } from "crm/funcs/organisations-com-crm-organisation-self-service-resource-list.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmOrganisationSelfServiceResourceList(crm, {
    id: "<id>",
    customFields: "key;value;key;value",
    distance: 5,
    lat: "\"35.1730837\"",
    lon: "\"33.3761312\"",
    name: "Bravo Coffee",
    tapCode: "01-23-45-67-89-AB",
    type: "MERCHANT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmOrganisationSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrganisationSelfServiceResourceListRequest](../../models/operations/com-crm-organisation-self-service-resource-list-request.md)                              | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrganisationSelfServiceResourceListResponse](../../models/operations/com-crm-organisation-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrganisationSelfServiceResourceSwitchOrganisation

Switch a contact’s access to another organisation that he/she is a member of

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrganisationSelfServiceResource_switchOrganisation" method="post" path="/self-service/v2/organisations/{id}/switch" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmOrganisationSelfServiceResourceSwitchOrganisation({
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
import { organisationsComCrmOrganisationSelfServiceResourceSwitchOrganisation } from "crm/funcs/organisations-com-crm-organisation-self-service-resource-switch-organisation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmOrganisationSelfServiceResourceSwitchOrganisation(crm, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmOrganisationSelfServiceResourceSwitchOrganisation failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrganisationSelfServiceResourceSwitchOrganisationRequest](../../models/operations/com-crm-organisation-self-service-resource-switch-organisation-request.md) | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrganisationSelfServiceResourceSwitchOrganisationResponse](../../models/operations/com-crm-organisation-self-service-resource-switch-organisation-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmMerchantSelfServiceResourceList

Search for organisations with active reward commercial terms that participate in one of the customer’s reward schemes

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.MerchantSelfServiceResource_list" method="get" path="/self-service/v2/rewards/merchants" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.organisations.comCrmMerchantSelfServiceResourceList({
    includeTotal: true,
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { organisationsComCrmMerchantSelfServiceResourceList } from "crm/funcs/organisations-com-crm-merchant-self-service-resource-list.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await organisationsComCrmMerchantSelfServiceResourceList(crm, {
    includeTotal: true,
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("organisationsComCrmMerchantSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmMerchantSelfServiceResourceListRequest](../../models/operations/com-crm-merchant-self-service-resource-list-request.md)                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmMerchantSelfServiceResourceListResponse](../../models/operations/com-crm-merchant-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |