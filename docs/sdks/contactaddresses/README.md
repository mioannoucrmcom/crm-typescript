# ContactAddresses

## Overview

Contact Addresses

### Available Operations

* [listContactAddressesSS](#listcontactaddressesss) - List Contact Addresses
* [addContactAddessSS](#addcontactaddessss) - Add Contact Address
* [updateContactAddressSS](#updatecontactaddressss) - Update Contact Address
* [deleteContactAddressSS](#deletecontactaddressss) - Delete Contact Address

## listContactAddressesSS

Retrieve all the addresses of a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="listContactAddressesSS" method="get" path="/self-service/v2/contacts/{id}/addresses" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAddresses.listContactAddressesSS({
    id: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactAddressesListContactAddressesSS } from "crmcom/funcs/contact-addresses-list-contact-addresses-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAddressesListContactAddressesSS(crmcom, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAddressesListContactAddressesSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ListContactAddressesSSRequest](../../models/operations/list-contact-addresses-ss-request.md)                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ListContactAddressesSSResponse](../../models/operations/list-contact-addresses-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## addContactAddessSS

Add a new address to an existing contact. A contact can have multiple addresses.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="addContactAddessSS" method="post" path="/self-service/v2/contacts/{id}/addresses" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAddresses.addContactAddessSS({
    id: "<id>",
    body: {
      type: "BUSINESS",
      isPrimary: true,
      addressLine1: "Elia Papakyriakou",
      addressLine2: "Tower Star",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2000",
      countryCode: "CYP",
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
import { contactAddressesAddContactAddessSS } from "crmcom/funcs/contact-addresses-add-contact-addess-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAddressesAddContactAddessSS(crmcom, {
    id: "<id>",
    body: {
      type: "BUSINESS",
      isPrimary: true,
      addressLine1: "Elia Papakyriakou",
      addressLine2: "Tower Star",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2000",
      countryCode: "CYP",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAddressesAddContactAddessSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AddContactAddessSSRequest](../../models/operations/add-contact-addess-ss-request.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AddContactAddessSSResponse](../../models/operations/add-contact-addess-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## updateContactAddressSS

Update one of the contact’s existing addresses

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateContactAddressSS" method="put" path="/self-service/v2/contacts/{id}/addresses/{address_id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAddresses.updateContactAddressSS({
    addressId: "cadbf723-fdc6-4598-8156-f6288e61f356",
    id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
    body: {
      type: "ALTERNATIVE",
      isPrimary: true,
      addressLine1: "Elia Papakyriakou",
      addressLine2: "Tower Star",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2000",
      countryCode: "CYP",
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
import { contactAddressesUpdateContactAddressSS } from "crmcom/funcs/contact-addresses-update-contact-address-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAddressesUpdateContactAddressSS(crmcom, {
    addressId: "cadbf723-fdc6-4598-8156-f6288e61f356",
    id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
    body: {
      type: "ALTERNATIVE",
      isPrimary: true,
      addressLine1: "Elia Papakyriakou",
      addressLine2: "Tower Star",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2000",
      countryCode: "CYP",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAddressesUpdateContactAddressSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateContactAddressSSRequest](../../models/operations/update-contact-address-ss-request.md)                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateContactAddressSSResponse](../../models/operations/update-contact-address-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## deleteContactAddressSS

Remove an existing address from a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteContactAddressSS" method="delete" path="/self-service/v2/contacts/{id}/addresses/{address_id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.contactAddresses.deleteContactAddressSS({
    addressId: "cadbf723-fdc6-4598-8156-f6288e61f356",
    id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactAddressesDeleteContactAddressSS } from "crmcom/funcs/contact-addresses-delete-contact-address-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAddressesDeleteContactAddressSS(crmcom, {
    addressId: "cadbf723-fdc6-4598-8156-f6288e61f356",
    id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactAddressesDeleteContactAddressSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteContactAddressSSRequest](../../models/operations/delete-contact-address-ss-request.md)                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |