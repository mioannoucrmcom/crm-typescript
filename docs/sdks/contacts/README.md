# Contacts

## Overview

Contacts are the customers of an organisation, the centre point of CRM.COM, and the starting point of any business flow.

### Available Operations

* [comCrmContactSelfServiceResourceGetContactSharedDevices](#comcrmcontactselfserviceresourcegetcontactshareddevices) - List Contact Shared Devices

## comCrmContactSelfServiceResourceGetContactSharedDevices

Returns all devices which were shared with a contact that is part of a community. By defaults all shared devices are returned

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactSharedDevices" method="get" path="/self-service/v2/contacts/{id}/communities/devices" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contacts.comCrmContactSelfServiceResourceGetContactSharedDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
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
import { contactsComCrmContactSelfServiceResourceGetContactSharedDevices } from "crm/funcs/contacts-com-crm-contact-self-service-resource-get-contact-shared-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactsComCrmContactSelfServiceResourceGetContactSharedDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactsComCrmContactSelfServiceResourceGetContactSharedDevices failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactSharedDevices" method="get" path="/self-service/v2/contacts/{id}/communities/devices" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contacts.comCrmContactSelfServiceResourceGetContactSharedDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
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
import { contactsComCrmContactSelfServiceResourceGetContactSharedDevices } from "crm/funcs/contacts-com-crm-contact-self-service-resource-get-contact-shared-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactsComCrmContactSelfServiceResourceGetContactSharedDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactsComCrmContactSelfServiceResourceGetContactSharedDevices failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactSharedDevices" method="get" path="/self-service/v2/contacts/{id}/communities/devices" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contacts.comCrmContactSelfServiceResourceGetContactSharedDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
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
import { contactsComCrmContactSelfServiceResourceGetContactSharedDevices } from "crm/funcs/contacts-com-crm-contact-self-service-resource-get-contact-shared-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactsComCrmContactSelfServiceResourceGetContactSharedDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactsComCrmContactSelfServiceResourceGetContactSharedDevices failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactSharedDevices" method="get" path="/self-service/v2/contacts/{id}/communities/devices" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contacts.comCrmContactSelfServiceResourceGetContactSharedDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
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
import { contactsComCrmContactSelfServiceResourceGetContactSharedDevices } from "crm/funcs/contacts-com-crm-contact-self-service-resource-get-contact-shared-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactsComCrmContactSelfServiceResourceGetContactSharedDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactsComCrmContactSelfServiceResourceGetContactSharedDevices failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                        | Type                                                                                                                                                                             | Required                                                                                                                                                                         | Description                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                        | [operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesRequest](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-request.md) | :heavy_check_mark:                                                                                                                                                               | The request object to use for the request.                                                                                                                                       |
| `options`                                                                                                                                                                        | RequestOptions                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                               | Used to set various options for making HTTP requests.                                                                                                                            |
| `options.fetchOptions`                                                                                                                                                           | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                          | :heavy_minus_sign:                                                                                                                                                               | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.   |
| `options.retries`                                                                                                                                                                | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                               | Enables retrying HTTP requests under certain failure conditions.                                                                                                                 |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesResponse](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |