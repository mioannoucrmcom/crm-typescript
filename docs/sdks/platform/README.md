# Platform

## Overview

Platform

### Available Operations

* [comCrmApplicationSelfServiceResourceGetApplication](#comcrmapplicationselfserviceresourcegetapplication) - Get Application
* [comCrmApplicationSelfServiceResourceList](#comcrmapplicationselfserviceresourcelist) - Integrations
* [comCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations](#comcrmapplicationselfserviceresourcegetapplicationembeddedlinkstranslations) - Get Application Embedded Links Translations
* [comCrmCustomFieldSelfServiceResourceListCustomFields](#comcrmcustomfieldselfserviceresourcelistcustomfields) - List Custom Fields
* [comCrmFileSelfServiceResourceGetFile](#comcrmfileselfserviceresourcegetfile) - Get File
* [comCrmFileSelfServiceResourceDeleteFile](#comcrmfileselfserviceresourcedeletefile) - Delete File
* [comCrmIndustrySelfServiceResourceListIndustries](#comcrmindustryselfserviceresourcelistindustries) - List Industries
* [comCrmLandingPageSelfServiceResourceGetSingleLandingPage](#comcrmlandingpageselfserviceresourcegetsinglelandingpage) - Get Landing Pages
* [comCrmLanguageSelfServiceResourceGetSupportedLanguages](#comcrmlanguageselfserviceresourcegetsupportedlanguages) - List Languages
* [comCrmSubIndustrySelfServiceResourceListSubIndustrySectors](#comcrmsubindustryselfserviceresourcelistsubindustrysectors) - List Sub-Industries
* [comCrmFileSelfServiceResourceUploadFile](#comcrmfileselfserviceresourceuploadfile) - Upload File

## comCrmApplicationSelfServiceResourceGetApplication

Retrieve details for a specific application

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApplicationSelfServiceResource_getApplication" method="get" path="/self-service/v2/applications" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.platform.comCrmApplicationSelfServiceResourceGetApplication({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    cloudName: "crm",
    platformAppId: "f9e4b742-bfe1-09dc-f623-de71aaed61ff",
    version: "\"1.1\"",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmApplicationSelfServiceResourceGetApplication } from "crmcom/funcs/platform-com-crm-application-self-service-resource-get-application.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await platformComCrmApplicationSelfServiceResourceGetApplication(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    cloudName: "crm",
    platformAppId: "f9e4b742-bfe1-09dc-f623-de71aaed61ff",
    version: "\"1.1\"",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmApplicationSelfServiceResourceGetApplication failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmApplicationSelfServiceResourceGetApplicationRequest](../../models/operations/com-crm-application-self-service-resource-get-application-request.md)           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmApplicationSelfServiceResourceGetApplicationSecurity](../../models/operations/com-crm-application-self-service-resource-get-application-security.md)         | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmApplicationSelfServiceResourceGetApplicationResponse](../../models/operations/com-crm-application-self-service-resource-get-application-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApplicationSelfServiceResourceList

Returns a list of supported (active) integrations for the specific application

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApplicationSelfServiceResource_list" method="get" path="/self-service/v2/applications/{id}/integrations" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmApplicationSelfServiceResourceList({
    id: "bd909bd2-2397-8af8-b256-87e496620209",
    connector: "JCC",
    finance: true,
    paymentMethod: "CARD",
    rewards: true,
    transactions: "PAYMENTS",
    type: "PAYMENT_GATEWAYS",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmApplicationSelfServiceResourceList } from "crmcom/funcs/platform-com-crm-application-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmApplicationSelfServiceResourceList(crmcom, {
    id: "bd909bd2-2397-8af8-b256-87e496620209",
    connector: "JCC",
    finance: true,
    paymentMethod: "CARD",
    rewards: true,
    transactions: "PAYMENTS",
    type: "PAYMENT_GATEWAYS",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmApplicationSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmApplicationSelfServiceResourceListRequest](../../models/operations/com-crm-application-self-service-resource-list-request.md)                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmApplicationSelfServiceResourceListResponse](../../models/operations/com-crm-application-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations

Retrieve translations of the embedded links for a specific application

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ApplicationSelfServiceResource_getApplicationEmbeddedLinksTranslations" method="get" path="/self-service/v2/applications/{id}/translations" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations({
    id: "bd909bd2-2397-8af8-b256-87e496620209",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  platformComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations,
} from "crmcom/funcs/platform-com-crm-application-self-service-resource-get-application-embedded-links-translations.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations(crmcom, {
    id: "bd909bd2-2397-8af8-b256-87e496620209",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                                 | Type                                                                                                                                                                                                                      | Required                                                                                                                                                                                                                  | Description                                                                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                                 | [operations.ComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslationsRequest](../../models/operations/com-crm-application-self-service-resource-get-application-embedded-links-translations-request.md) | :heavy_check_mark:                                                                                                                                                                                                        | The request object to use for the request.                                                                                                                                                                                |
| `options`                                                                                                                                                                                                                 | RequestOptions                                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                        | Used to set various options for making HTTP requests.                                                                                                                                                                     |
| `options.fetchOptions`                                                                                                                                                                                                    | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                                        | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                            |
| `options.retries`                                                                                                                                                                                                         | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                                        | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                          |

### Response

**Promise\<[operations.ComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslationsResponse](../../models/operations/com-crm-application-self-service-resource-get-application-embedded-links-translations-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmCustomFieldSelfServiceResourceListCustomFields

eturns a list of custom fields configured in the system as “enabled” and “visible for self-service”

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.CustomFieldSelfServiceResource_listCustomFields" method="get" path="/self-service/v2/custom_fields" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.platform.comCrmCustomFieldSelfServiceResourceListCustomFields({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmCustomFieldSelfServiceResourceListCustomFields } from "crmcom/funcs/platform-com-crm-custom-field-self-service-resource-list-custom-fields.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await platformComCrmCustomFieldSelfServiceResourceListCustomFields(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmCustomFieldSelfServiceResourceListCustomFields failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmCustomFieldSelfServiceResourceListCustomFieldsRequest](../../models/operations/com-crm-custom-field-self-service-resource-list-custom-fields-request.md)     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmCustomFieldSelfServiceResourceListCustomFieldsSecurity](../../models/operations/com-crm-custom-field-self-service-resource-list-custom-fields-security.md)   | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmCustomFieldSelfServiceResourceListCustomFieldsResponse](../../models/operations/com-crm-custom-field-self-service-resource-list-custom-fields-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmFileSelfServiceResourceGetFile

Retrieve a specific file (response will return the actual file)

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.FileSelfServiceResource_getFile" method="get" path="/self-service/v2/files/{id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.platform.comCrmFileSelfServiceResourceGetFile({
    id: "3ae9d64a-8a3b-f1e1-eed6-05b307f926fb",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmFileSelfServiceResourceGetFile } from "crmcom/funcs/platform-com-crm-file-self-service-resource-get-file.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmFileSelfServiceResourceGetFile(crmcom, {
    id: "3ae9d64a-8a3b-f1e1-eed6-05b307f926fb",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("platformComCrmFileSelfServiceResourceGetFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmFileSelfServiceResourceGetFileRequest](../../models/operations/com-crm-file-self-service-resource-get-file-request.md)                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmFileSelfServiceResourceDeleteFile

Delete a file

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.FileSelfServiceResource_deleteFile" method="delete" path="/self-service/v2/files/{id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.platform.comCrmFileSelfServiceResourceDeleteFile({
    id: "8dfc2223-edca-f05d-820b-dc96ba9df2c2",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmFileSelfServiceResourceDeleteFile } from "crmcom/funcs/platform-com-crm-file-self-service-resource-delete-file.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmFileSelfServiceResourceDeleteFile(crmcom, {
    id: "8dfc2223-edca-f05d-820b-dc96ba9df2c2",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("platformComCrmFileSelfServiceResourceDeleteFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmFileSelfServiceResourceDeleteFileRequest](../../models/operations/com-crm-file-self-service-resource-delete-file-request.md)                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmIndustrySelfServiceResourceListIndustries

Returns a list of industries

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.IndustrySelfServiceResource_listIndustries" method="get" path="/self-service/v2/industries" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmIndustrySelfServiceResourceListIndustries({
    name: "Education",
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmIndustrySelfServiceResourceListIndustries } from "crmcom/funcs/platform-com-crm-industry-self-service-resource-list-industries.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmIndustrySelfServiceResourceListIndustries(crmcom, {
    name: "Education",
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmIndustrySelfServiceResourceListIndustries failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.IndustrySelfServiceResource_listIndustries" method="get" path="/self-service/v2/industries" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmIndustrySelfServiceResourceListIndustries({
    name: "Education",
    page: 20,
    size: 20,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmIndustrySelfServiceResourceListIndustries } from "crmcom/funcs/platform-com-crm-industry-self-service-resource-list-industries.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmIndustrySelfServiceResourceListIndustries(crmcom, {
    name: "Education",
    page: 20,
    size: 20,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmIndustrySelfServiceResourceListIndustries failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.IndustrySelfServiceResource_listIndustries" method="get" path="/self-service/v2/industries" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmIndustrySelfServiceResourceListIndustries({
    name: "Education",
    page: 20,
    size: 20,
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
import { platformComCrmIndustrySelfServiceResourceListIndustries } from "crmcom/funcs/platform-com-crm-industry-self-service-resource-list-industries.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmIndustrySelfServiceResourceListIndustries(crmcom, {
    name: "Education",
    page: 20,
    size: 20,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmIndustrySelfServiceResourceListIndustries failed:", res.error);
  }
}

run();
```
### Example Usage: POSTED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.IndustrySelfServiceResource_listIndustries" method="get" path="/self-service/v2/industries" example="POSTED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmIndustrySelfServiceResourceListIndustries({
    name: "Education",
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmIndustrySelfServiceResourceListIndustries } from "crmcom/funcs/platform-com-crm-industry-self-service-resource-list-industries.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmIndustrySelfServiceResourceListIndustries(crmcom, {
    name: "Education",
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmIndustrySelfServiceResourceListIndustries failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.IndustrySelfServiceResource_listIndustries" method="get" path="/self-service/v2/industries" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmIndustrySelfServiceResourceListIndustries({
    name: "Education",
    page: 20,
    size: 20,
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
import { platformComCrmIndustrySelfServiceResourceListIndustries } from "crmcom/funcs/platform-com-crm-industry-self-service-resource-list-industries.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmIndustrySelfServiceResourceListIndustries(crmcom, {
    name: "Education",
    page: 20,
    size: 20,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmIndustrySelfServiceResourceListIndustries failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmIndustrySelfServiceResourceListIndustriesRequest](../../models/operations/com-crm-industry-self-service-resource-list-industries-request.md)                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmIndustrySelfServiceResourceListIndustriesResponse](../../models/operations/com-crm-industry-self-service-resource-list-industries-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmLandingPageSelfServiceResourceGetSingleLandingPage

This request returns the details and design of the landing page requested.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.LandingPageSelfServiceResource_getSingleLandingPage" method="get" path="/self-service/v2/landing_pages/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmLandingPageSelfServiceResourceGetSingleLandingPage({
    id: "JHGDFJHGSF6576GHFDSHG",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmLandingPageSelfServiceResourceGetSingleLandingPage } from "crmcom/funcs/platform-com-crm-landing-page-self-service-resource-get-single-landing-page.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmLandingPageSelfServiceResourceGetSingleLandingPage(crmcom, {
    id: "JHGDFJHGSF6576GHFDSHG",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmLandingPageSelfServiceResourceGetSingleLandingPage failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                           | Type                                                                                                                                                                                | Required                                                                                                                                                                            | Description                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                           | [operations.ComCrmLandingPageSelfServiceResourceGetSingleLandingPageRequest](../../models/operations/com-crm-landing-page-self-service-resource-get-single-landing-page-request.md) | :heavy_check_mark:                                                                                                                                                                  | The request object to use for the request.                                                                                                                                          |
| `options`                                                                                                                                                                           | RequestOptions                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                  | Used to set various options for making HTTP requests.                                                                                                                               |
| `options.fetchOptions`                                                                                                                                                              | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                             | :heavy_minus_sign:                                                                                                                                                                  | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.      |
| `options.retries`                                                                                                                                                                   | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                  | Enables retrying HTTP requests under certain failure conditions.                                                                                                                    |

### Response

**Promise\<[operations.ComCrmLandingPageSelfServiceResourceGetSingleLandingPageResponse](../../models/operations/com-crm-landing-page-self-service-resource-get-single-landing-page-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmLanguageSelfServiceResourceGetSupportedLanguages

Retrieve a list of the supported languages that can be used in communications and content translations
<div class="spec-item-section">
                                    <h4>Notes</h4>
                                    <div class="description spec-item-section__description"><div class="callout callout-info"><div class="callout-header"><strong>COMMUNICATION &amp; CONTENT TRANSLATION LANGUAGES</strong></div><p>Communication languages can be configured per business and are used for sending a communication content or display an entity’s content in different languages (based on contact’s preferred communication language).</p>
</div>
</div></div>

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.LanguageSelfServiceResource_getSupportedLanguages" method="get" path="/self-service/v2/languages" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmLanguageSelfServiceResourceGetSupportedLanguages();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmLanguageSelfServiceResourceGetSupportedLanguages } from "crmcom/funcs/platform-com-crm-language-self-service-resource-get-supported-languages.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmLanguageSelfServiceResourceGetSupportedLanguages(crmcom);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmLanguageSelfServiceResourceGetSupportedLanguages failed:", res.error);
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

**Promise\<[operations.ComCrmLanguageSelfServiceResourceGetSupportedLanguagesResponse](../../models/operations/com-crm-language-self-service-resource-get-supported-languages-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSubIndustrySelfServiceResourceListSubIndustrySectors

Returns a list of sub-industries

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubIndustrySelfServiceResource_listSubIndustrySectors" method="get" path="/self-service/v2/sub_industries" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmSubIndustrySelfServiceResourceListSubIndustrySectors({
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors } from "crmcom/funcs/platform-com-crm-sub-industry-self-service-resource-list-sub-industry-sectors.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors(crmcom, {
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
    sort: "CREATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.SubIndustrySelfServiceResource_listSubIndustrySectors" method="get" path="/self-service/v2/sub_industries" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmSubIndustrySelfServiceResourceListSubIndustrySectors({
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors } from "crmcom/funcs/platform-com-crm-sub-industry-self-service-resource-list-sub-industry-sectors.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors(crmcom, {
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SubIndustrySelfServiceResource_listSubIndustrySectors" method="get" path="/self-service/v2/sub_industries" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmSubIndustrySelfServiceResourceListSubIndustrySectors({
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
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
import { platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors } from "crmcom/funcs/platform-com-crm-sub-industry-self-service-resource-list-sub-industry-sectors.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors(crmcom, {
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors failed:", res.error);
  }
}

run();
```
### Example Usage: POSTED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubIndustrySelfServiceResource_listSubIndustrySectors" method="get" path="/self-service/v2/sub_industries" example="POSTED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmSubIndustrySelfServiceResourceListSubIndustrySectors({
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors } from "crmcom/funcs/platform-com-crm-sub-industry-self-service-resource-list-sub-industry-sectors.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors(crmcom, {
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
    sort: "POSTED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SubIndustrySelfServiceResource_listSubIndustrySectors" method="get" path="/self-service/v2/sub_industries" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmSubIndustrySelfServiceResourceListSubIndustrySectors({
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
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
import { platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors } from "crmcom/funcs/platform-com-crm-sub-industry-self-service-resource-list-sub-industry-sectors.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors(crmcom, {
    industryName: "EDUCATION",
    name: "RESTAURANTS",
    page: 20,
    size: 20,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                               | Type                                                                                                                                                                                    | Required                                                                                                                                                                                | Description                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                               | [operations.ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsRequest](../../models/operations/com-crm-sub-industry-self-service-resource-list-sub-industry-sectors-request.md) | :heavy_check_mark:                                                                                                                                                                      | The request object to use for the request.                                                                                                                                              |
| `options`                                                                                                                                                                               | RequestOptions                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                      | Used to set various options for making HTTP requests.                                                                                                                                   |
| `options.fetchOptions`                                                                                                                                                                  | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                 | :heavy_minus_sign:                                                                                                                                                                      | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.          |
| `options.retries`                                                                                                                                                                       | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                      | Enables retrying HTTP requests under certain failure conditions.                                                                                                                        |

### Response

**Promise\<[operations.ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsResponse](../../models/operations/com-crm-sub-industry-self-service-resource-list-sub-industry-sectors-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmFileSelfServiceResourceUploadFile

Create an upload signature for files. Uploading files into CRM.COM is achieved firstly by creating a signature for the file that will be uploaded and then connecting it to the related entity, e.g. Service Request (using the respective entity file APIs).

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.FileSelfServiceResource_uploadFile" method="post" path="/self-service/v2/upload/files" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";
import { openAsBlob } from "node:fs";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.platform.comCrmFileSelfServiceResourceUploadFile({
    file: await openAsBlob("example.file"),
    fileEntityType: "ORDERS",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { platformComCrmFileSelfServiceResourceUploadFile } from "crmcom/funcs/platform-com-crm-file-self-service-resource-upload-file.js";
import { openAsBlob } from "node:fs";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await platformComCrmFileSelfServiceResourceUploadFile(crmcom, {
    file: await openAsBlob("example.file"),
    fileEntityType: "ORDERS",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("platformComCrmFileSelfServiceResourceUploadFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmFileSelfServiceResourceUploadFileRequest](../../models/operations/com-crm-file-self-service-resource-upload-file-request.md)                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmFileSelfServiceResourceUploadFileResponse](../../models/operations/com-crm-file-self-service-resource-upload-file-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |