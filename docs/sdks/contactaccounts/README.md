# ContactAccounts

## Overview

Contact Accounts

### Available Operations

* [comCrmAccountSelfServiceResourceGetSingle](#comcrmaccountselfserviceresourcegetsingle) - Get Account
* [comCrmAccountSelfServiceResourceUpdateAccount](#comcrmaccountselfserviceresourceupdateaccount) - Update Account
* [comCrmAccountSelfServiceResourceListAccountJournals](#comcrmaccountselfserviceresourcelistaccountjournals) - List Account Journals
* [comCrmAccountSelfServiceResourceList](#comcrmaccountselfserviceresourcelist) - List Contact Accounts
* [comCrmAccountSelfServiceResourceAddContactAccount](#comcrmaccountselfserviceresourceaddcontactaccount) - Create account
* [comCrmAccountSelfServiceResourceGetAccountJournal](#comcrmaccountselfserviceresourcegetaccountjournal) - Get Account Journal

## comCrmAccountSelfServiceResourceGetSingle

Retrieve details and financial information for an account

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_getSingle" method="get" path="/self-service/v2/accounts/{id}" example="Get Account response" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceGetSingle({
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
import { contactAccountsComCrmAccountSelfServiceResourceGetSingle } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-get-single.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceGetSingle(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceGetSingleRequest](../../models/operations/com-crm-account-self-service-resource-get-single-request.md)                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAccountSelfServiceResourceGetSingleResponse](../../models/operations/com-crm-account-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAccountSelfServiceResourceUpdateAccount

Update an existing account of a contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_updateAccount" method="put" path="/self-service/v2/accounts/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceUpdateAccount({
    id: "AF1D8C778F6540E29EECEABCD8711C3A",
    body: {
      classificationId: "8F95E1B6FEC1487E88A9AAF3C214A870",
      isPrimary: true,
      billingAddressId: "974A084BA7794F6D9A2F94A521DDCDAB",
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
import { contactAccountsComCrmAccountSelfServiceResourceUpdateAccount } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-update-account.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceUpdateAccount(crmcom, {
    id: "AF1D8C778F6540E29EECEABCD8711C3A",
    body: {
      classificationId: "8F95E1B6FEC1487E88A9AAF3C214A870",
      isPrimary: true,
      billingAddressId: "974A084BA7794F6D9A2F94A521DDCDAB",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceUpdateAccount failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceUpdateAccountRequest](../../models/operations/com-crm-account-self-service-resource-update-account-request.md)                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAccountSelfServiceResourceUpdateAccountResponse](../../models/operations/com-crm-account-self-service-resource-update-account-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAccountSelfServiceResourceListAccountJournals

Retrieve a list of account journals. Only journals with Posted transactions are returned. By default, accounts journals of the last 12 months are retrieved.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: posted_on[gt]

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="posted_on[gt]" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: posted_on[gte]

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="posted_on[gte]" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: posted_on[lt]

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="posted_on[lt]" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```
### Example Usage: posted_on[lte]

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_listAccountJournals" method="get" path="/self-service/v2/accounts/{id}/journals" example="posted_on[lte]" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceListAccountJournals({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
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
import { contactAccountsComCrmAccountSelfServiceResourceListAccountJournals } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list-account-journals.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceListAccountJournals(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    transactionType: "INVOICE",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceListAccountJournals failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceListAccountJournalsRequest](../../models/operations/com-crm-account-self-service-resource-list-account-journals-request.md)        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAccountSelfServiceResourceListAccountJournalsResponse](../../models/operations/com-crm-account-self-service-resource-list-account-journals-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAccountSelfServiceResourceList

Get a list of Contact Accounts. Normally a contact will have a single account but multiple accounts can be used to service different currencies, or different spending profiles.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/accounts" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
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
import { contactAccountsComCrmAccountSelfServiceResourceList } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/accounts" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
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
import { contactAccountsComCrmAccountSelfServiceResourceList } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/accounts" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
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
import { contactAccountsComCrmAccountSelfServiceResourceList } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/accounts" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
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
import { contactAccountsComCrmAccountSelfServiceResourceList } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_list" method="get" path="/self-service/v2/contacts/{id}/accounts" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceList({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
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
import { contactAccountsComCrmAccountSelfServiceResourceList } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceList(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    currencyCode: "EUR",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceListRequest](../../models/operations/com-crm-account-self-service-resource-list-request.md)                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAccountSelfServiceResourceListResponse](../../models/operations/com-crm-account-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAccountSelfServiceResourceAddContactAccount

Add a new customer account to an existing contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_addContactAccount" method="post" path="/self-service/v2/contacts/{id}/accounts" example="Add Account for Contact" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceAddContactAccount({
    id: "<id>",
    body: {
      classificationId: "dfa582fa-9c68-4f6c-ae78-52a51098155e",
      currencyCode: "EUR",
      isPrimary: false,
      billingAddressId: "e12c4256-b9ba-47c2-970a-bb47628c1600",
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
import { contactAccountsComCrmAccountSelfServiceResourceAddContactAccount } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-add-contact-account.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceAddContactAccount(crmcom, {
    id: "<id>",
    body: {
      classificationId: "dfa582fa-9c68-4f6c-ae78-52a51098155e",
      currencyCode: "EUR",
      isPrimary: false,
      billingAddressId: "e12c4256-b9ba-47c2-970a-bb47628c1600",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceAddContactAccount failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceAddContactAccountRequest](../../models/operations/com-crm-account-self-service-resource-add-contact-account-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAccountSelfServiceResourceAddContactAccountResponse](../../models/operations/com-crm-account-self-service-resource-add-contact-account-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAccountSelfServiceResourceGetAccountJournal

Retrieve information and details lines for a single account journal.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_getAccountJournal" method="get" path="/self-service/v2/journals/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts.comCrmAccountSelfServiceResourceGetAccountJournal({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    includeLines: false,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactAccountsComCrmAccountSelfServiceResourceGetAccountJournal } from "crmcom/funcs/contact-accounts-com-crm-account-self-service-resource-get-account-journal.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAccountsComCrmAccountSelfServiceResourceGetAccountJournal(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    includeLines: false,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAccountsComCrmAccountSelfServiceResourceGetAccountJournal failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceGetAccountJournalRequest](../../models/operations/com-crm-account-self-service-resource-get-account-journal-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAccountSelfServiceResourceGetAccountJournalResponse](../../models/operations/com-crm-account-self-service-resource-get-account-journal-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |