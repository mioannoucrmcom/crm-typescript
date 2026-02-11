# Donations

## Overview

Donations

### Available Operations

* [comCrmRewardOfferDonationsSelfServiceResourceList](#comcrmrewardofferdonationsselfserviceresourcelist) - Search Donation Offers
* [comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs](#comcrmrewardofferdonationsselfserviceresourcelistcharityorgs) - List Charity Organisations
* [comCrmRewardOfferDonationsSelfServiceResourceGetSingle](#comcrmrewardofferdonationsselfserviceresourcegetsingle) - Get Donation Offer

## comCrmRewardOfferDonationsSelfServiceResourceList

Retrieve a list of Donation offers to which a contact can opt in and start making donations to various organisations. Only Active Donation offers are returned (offers still within their validity periods). For additional information for each offer, a sub-sequent call to "GET Reward Offer" can be used.

### Example Usage: BUNDLE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="BUNDLE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
    types: "BUNDLE",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    types: "BUNDLE",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: DISCOUNT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="DISCOUNT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
    types: "DISCOUNT",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    types: "DISCOUNT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: GIFT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="GIFT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
    types: "GIFT",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    types: "GIFT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: ONE_OFF

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="ONE_OFF" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
    types: "ONE_OFF",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    types: "ONE_OFF",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: PER_TRANSACTION

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="PER_TRANSACTION" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    donationTypes: "PER_TRANSACTION",
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    donationTypes: "PER_TRANSACTION",
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: TERMED

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="TERMED" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    donationTypes: "TERMED",
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    donationTypes: "TERMED",
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: VARIABLE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_list" method="get" path="/self-service/v2/donation_offers" example="VARIABLE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceList({
    donationTypes: "VARIABLE",
    searchValue: "Increase Visits",
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
import { donationsComCrmRewardOfferDonationsSelfServiceResourceList } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceList(crmcom, {
    donationTypes: "VARIABLE",
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmRewardOfferDonationsSelfServiceResourceListRequest](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmRewardOfferDonationsSelfServiceResourceListResponse](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs

Returns a list of Organisations (B2B Merchants of the Business) for which a Donation offer is configured so as contact can make donations to these Organisations. By default, only Organisations with Active (and still valid) Donation Offers are returned.

### Example Usage: BUNDLE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_listCharityOrgs" method="get" path="/self-service/v2/donation_offers/organisations" example="BUNDLE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs({
    includeCreatives: true,
    type: "BUNDLE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list-charity-orgs.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs(crmcom, {
    includeCreatives: true,
    type: "BUNDLE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs failed:", res.error);
  }
}

run();
```
### Example Usage: DISCOUNT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_listCharityOrgs" method="get" path="/self-service/v2/donation_offers/organisations" example="DISCOUNT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs({
    includeCreatives: true,
    type: "DISCOUNT",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list-charity-orgs.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs(crmcom, {
    includeCreatives: true,
    type: "DISCOUNT",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_listCharityOrgs" method="get" path="/self-service/v2/donation_offers/organisations" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs({
    includeCreatives: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list-charity-orgs.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs(crmcom, {
    includeCreatives: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs failed:", res.error);
  }
}

run();
```
### Example Usage: GIFT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_listCharityOrgs" method="get" path="/self-service/v2/donation_offers/organisations" example="GIFT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs({
    includeCreatives: true,
    type: "GIFT",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list-charity-orgs.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs(crmcom, {
    includeCreatives: true,
    type: "GIFT",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs failed:", res.error);
  }
}

run();
```
### Example Usage: ONE_OFF

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_listCharityOrgs" method="get" path="/self-service/v2/donation_offers/organisations" example="ONE_OFF" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs({
    includeCreatives: true,
    type: "ONE_OFF",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-list-charity-orgs.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs(crmcom, {
    includeCreatives: true,
    type: "ONE_OFF",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                   | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                   | [operations.ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsRequest](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-charity-orgs-request.md) | :heavy_check_mark:                                                                                                                                                                          | The request object to use for the request.                                                                                                                                                  |
| `options`                                                                                                                                                                                   | RequestOptions                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                          | Used to set various options for making HTTP requests.                                                                                                                                       |
| `options.fetchOptions`                                                                                                                                                                      | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                     | :heavy_minus_sign:                                                                                                                                                                          | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.              |
| `options.retries`                                                                                                                                                                           | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                          | Enables retrying HTTP requests under certain failure conditions.                                                                                                                            |

### Response

**Promise\<[operations.ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsResponse](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-charity-orgs-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmRewardOfferDonationsSelfServiceResourceGetSingle

Retrieve detailed information for a donation offer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferDonationsSelfServiceResource_getSingle" method="get" path="/self-service/v2/donation_offers/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.donations.comCrmRewardOfferDonationsSelfServiceResourceGetSingle({
    id: "6883441e-194a-b92b-c6c0-2f0e869e4c65",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { donationsComCrmRewardOfferDonationsSelfServiceResourceGetSingle } from "crmcom/funcs/donations-com-crm-reward-offer-donations-self-service-resource-get-single.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await donationsComCrmRewardOfferDonationsSelfServiceResourceGetSingle(crmcom, {
    id: "6883441e-194a-b92b-c6c0-2f0e869e4c65",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("donationsComCrmRewardOfferDonationsSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmRewardOfferDonationsSelfServiceResourceGetSingleRequest](../../models/operations/com-crm-reward-offer-donations-self-service-resource-get-single-request.md) | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmRewardOfferDonationsSelfServiceResourceGetSingleResponse](../../models/operations/com-crm-reward-offer-donations-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |