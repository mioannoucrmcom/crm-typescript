# ContactAttachments

## Overview

Contact Attachments

### Available Operations

* [comCrmContactSelfServiceResourceGetFiles](#comcrmcontactselfserviceresourcegetfiles) - List Contact Attachments
* [comCrmContactSelfServiceResourceCreateFile](#comcrmcontactselfserviceresourcecreatefile) - Add Contact Attachment
* [comCrmContactSelfServiceResourceRemoveFile](#comcrmcontactselfserviceresourceremovefile) - Delete Contact Attachment

## comCrmContactSelfServiceResourceGetFiles

Retrieve all attachment files for a specific contact

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getFiles" method="get" path="/self-service/v2/contacts/{id}/attachments" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactAttachments.comCrmContactSelfServiceResourceGetFiles({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { contactAttachmentsComCrmContactSelfServiceResourceGetFiles } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-get-files.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceGetFiles(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: List Contact Files

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getFiles" method="get" path="/self-service/v2/contacts/{id}/attachments" example="List Contact Files" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactAttachments.comCrmContactSelfServiceResourceGetFiles({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { contactAttachmentsComCrmContactSelfServiceResourceGetFiles } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-get-files.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceGetFiles(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getFiles" method="get" path="/self-service/v2/contacts/{id}/attachments" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactAttachments.comCrmContactSelfServiceResourceGetFiles({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { contactAttachmentsComCrmContactSelfServiceResourceGetFiles } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-get-files.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceGetFiles(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getFiles" method="get" path="/self-service/v2/contacts/{id}/attachments" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactAttachments.comCrmContactSelfServiceResourceGetFiles({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { contactAttachmentsComCrmContactSelfServiceResourceGetFiles } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-get-files.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceGetFiles(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getFiles" method="get" path="/self-service/v2/contacts/{id}/attachments" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactAttachments.comCrmContactSelfServiceResourceGetFiles({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { contactAttachmentsComCrmContactSelfServiceResourceGetFiles } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-get-files.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceGetFiles(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceGetFiles failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetFilesRequest](../../models/operations/com-crm-contact-self-service-resource-get-files-request.md)                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceGetFilesSecurity](../../models/operations/com-crm-contact-self-service-resource-get-files-security.md)                             | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetFilesResponse](../../models/operations/com-crm-contact-self-service-resource-get-files-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceCreateFile

Add an attachment (file or link) to an existing contact. Adding a file attachment is achieved firstly by creating a signature for the file that will be uploaded and then connecting it to the related contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_createFile" method="post" path="/self-service/v2/contacts/{id}/attachments" example="Add Contact File" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactAttachments.comCrmContactSelfServiceResourceCreateFile({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      fileId: "30526723-24a3-e4e3-1a75-b26b1b41f05c",
      link: "https://crmcom.sharepoint.com/:x:/s/contacts/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
      description: "Screenshot sent by contact",
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
import { contactAttachmentsComCrmContactSelfServiceResourceCreateFile } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-create-file.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceCreateFile(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    body: {
      fileId: "30526723-24a3-e4e3-1a75-b26b1b41f05c",
      link: "https://crmcom.sharepoint.com/:x:/s/contacts/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
      description: "Screenshot sent by contact",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceCreateFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceCreateFileRequest](../../models/operations/com-crm-contact-self-service-resource-create-file-request.md)                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceCreateFileSecurity](../../models/operations/com-crm-contact-self-service-resource-create-file-security.md)                         | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceCreateFileResponse](../../models/operations/com-crm-contact-self-service-resource-create-file-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceRemoveFile

Delete a specific contact's attachment

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_removeFile" method="delete" path="/self-service/v2/contacts/{id}/attachments/{attachment_id}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  await crm.contactAttachments.comCrmContactSelfServiceResourceRemoveFile({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    attachmentId: "<id>",
    id: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAttachmentsComCrmContactSelfServiceResourceRemoveFile } from "crm/funcs/contact-attachments-com-crm-contact-self-service-resource-remove-file.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactAttachmentsComCrmContactSelfServiceResourceRemoveFile(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    attachmentId: "<id>",
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactAttachmentsComCrmContactSelfServiceResourceRemoveFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceRemoveFileRequest](../../models/operations/com-crm-contact-self-service-resource-remove-file-request.md)                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceRemoveFileSecurity](../../models/operations/com-crm-contact-self-service-resource-remove-file-security.md)                         | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |