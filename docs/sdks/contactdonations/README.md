# ContactDonations

## Overview

Contact Donations

### Available Operations

* [comCrmContactSelfServiceResourceListContactDonations](#comcrmcontactselfserviceresourcelistcontactdonations) - List Contact Donation Offers
* [comCrmContactSelfServiceResourceOptInDonations](#comcrmcontactselfserviceresourceoptindonations) - Contact Donation Actions
* [comCrmContactDonationSelfServiceResourceListContactDonationsHistory](#comcrmcontactdonationselfserviceresourcelistcontactdonationshistory) - List Contact Donation Offers History
* [comCrmContactSelfServiceResourceUpdateDonations](#comcrmcontactselfserviceresourceupdatedonations) - Update donation offer preferences
* [comCrmContactSelfServiceResourceOptOutDonations](#comcrmcontactselfserviceresourceoptoutdonations) - Opt out from Donation offer

## comCrmContactSelfServiceResourceListContactDonations

By default returns a list of donations to which the contact is currenlty opt-in. Optionally, the Web API can be used to additionally retrieve any donation offers to which the contact has opted-out from.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_listContactDonations" method="get" path="/self-service/v2/contacts/{id}/donations" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDonations.comCrmContactSelfServiceResourceListContactDonations({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    includeOptOut: true,
    includeTotal: true,
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactDonationsComCrmContactSelfServiceResourceListContactDonations } from "crm/funcs/contact-donations-com-crm-contact-self-service-resource-list-contact-donations.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDonationsComCrmContactSelfServiceResourceListContactDonations(crm, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    includeOptOut: true,
    includeTotal: true,
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDonationsComCrmContactSelfServiceResourceListContactDonations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceListContactDonationsRequest](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-request.md)      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceListContactDonationsResponse](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceOptInDonations

Use Web API whenever a contact wants to opt-in to a Donation offer. Once opt-in, a new Donation is made automatically either on each contact purchase or on a termed basis, depending on the donation offer to which the contact opted-in. Contact might opt-in to various Donation offers and can opt-out at any point of time.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_optInDonations" method="post" path="/self-service/v2/contacts/{id}/donations" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactDonations.comCrmContactSelfServiceResourceOptInDonations({
    id: "<id>",
    body: {
      donationOfferId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      multiplier: 2,
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactDonationsComCrmContactSelfServiceResourceOptInDonations } from "crm/funcs/contact-donations-com-crm-contact-self-service-resource-opt-in-donations.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDonationsComCrmContactSelfServiceResourceOptInDonations(crm, {
    id: "<id>",
    body: {
      donationOfferId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      multiplier: 2,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactDonationsComCrmContactSelfServiceResourceOptInDonations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceOptInDonationsRequest](../../models/operations/com-crm-contact-self-service-resource-opt-in-donations-request.md)                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactDonationSelfServiceResourceListContactDonationsHistory

Returns a list of donations made by the contact so far.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactDonationSelfServiceResource_listContactDonationsHistory" method="get" path="/self-service/v2/contacts/{id}/donations/history" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDonations.comCrmContactDonationSelfServiceResourceListContactDonationsHistory({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    includeTotal: true,
    organisationId: "3afad71d-e015-4e98-a464-f438c93edcde",
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import {
  contactDonationsComCrmContactDonationSelfServiceResourceListContactDonationsHistory,
} from "crm/funcs/contact-donations-com-crm-contact-donation-self-service-resource-list-contact-donations-history.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDonationsComCrmContactDonationSelfServiceResourceListContactDonationsHistory(crm, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    includeTotal: true,
    organisationId: "3afad71d-e015-4e98-a464-f438c93edcde",
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDonationsComCrmContactDonationSelfServiceResourceListContactDonationsHistory failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                 | Type                                                                                                                                                                                                      | Required                                                                                                                                                                                                  | Description                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                 | [operations.ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryRequest](../../models/operations/com-crm-contact-donation-self-service-resource-list-contact-donations-history-request.md) | :heavy_check_mark:                                                                                                                                                                                        | The request object to use for the request.                                                                                                                                                                |
| `options`                                                                                                                                                                                                 | RequestOptions                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                        | Used to set various options for making HTTP requests.                                                                                                                                                     |
| `options.fetchOptions`                                                                                                                                                                                    | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                        | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                            |
| `options.retries`                                                                                                                                                                                         | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                        | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                          |

### Response

**Promise\<[operations.ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryResponse](../../models/operations/com-crm-contact-donation-self-service-resource-list-contact-donations-history-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceUpdateDonations

Update a contact's preferences for the donations to which they opted-in. Only one of the request parameters can be updated in each Web API call. Only donation offers to which the contact is currently opted-in can be updated.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_updateDonations" method="put" path="/self-service/v2/contacts/{id}/donations/{donation_id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactDonations.comCrmContactSelfServiceResourceUpdateDonations({
    donationId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    id: "5096c4d4-c387-9888-d631-80e74546e2db",
    body: {
      donationOfferId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      multiplier: 2,
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactDonationsComCrmContactSelfServiceResourceUpdateDonations } from "crm/funcs/contact-donations-com-crm-contact-self-service-resource-update-donations.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDonationsComCrmContactSelfServiceResourceUpdateDonations(crm, {
    donationId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    id: "5096c4d4-c387-9888-d631-80e74546e2db",
    body: {
      donationOfferId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      multiplier: 2,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactDonationsComCrmContactSelfServiceResourceUpdateDonations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceUpdateDonationsRequest](../../models/operations/com-crm-contact-self-service-resource-update-donations-request.md)                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceOptOutDonations

Opts-out a contact from a donation offer. Only donation offers to which the contact is currenlty opted-in can be removed.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_optOutDonations" method="delete" path="/self-service/v2/contacts/{id}/donations/{donation_id}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactDonations.comCrmContactSelfServiceResourceOptOutDonations({
    donationId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    id: "5096c4d4-c387-9888-d631-80e74546e2db",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactDonationsComCrmContactSelfServiceResourceOptOutDonations } from "crm/funcs/contact-donations-com-crm-contact-self-service-resource-opt-out-donations.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDonationsComCrmContactSelfServiceResourceOptOutDonations(crm, {
    donationId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    id: "5096c4d4-c387-9888-d631-80e74546e2db",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactDonationsComCrmContactSelfServiceResourceOptOutDonations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceOptOutDonationsRequest](../../models/operations/com-crm-contact-self-service-resource-opt-out-donations-request.md)                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |