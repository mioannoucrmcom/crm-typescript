# ContactDevices

## Overview

The (Contact Devices) APIs are updated to cover a significant number of use cases where devices can be associated with a contact. For backwards compatibility, the attribute ‘registration_type’ (including its enum values) is still operational, but on the new design is listed as ‘platform’.

### Available Operations

* [comCrmDeviceSelfServiceResourceGetContactDevices](#comcrmdeviceselfserviceresourcegetcontactdevices) - List Devices
* [comCrmDeviceSelfServiceResourceAddContactDevice](#comcrmdeviceselfserviceresourceaddcontactdevice) - Register Device
* [comCrmDeviceSelfServiceResourceListDeviceMeterReadings](#comcrmdeviceselfserviceresourcelistdevicemeterreadings) - List Device Meter Readings
* [comCrmDeviceSelfServiceResourceCreateDeviceMeterReading](#comcrmdeviceselfserviceresourcecreatedevicemeterreading) - Create Device Meter Reading
* [comCrmDeviceSelfServiceResourceRemoveContactDevice](#comcrmdeviceselfserviceresourceremovecontactdevice) - Delete Contact Devices
* [comCrmDeviceSelfServiceResourceUpdateDevice](#comcrmdeviceselfserviceresourceupdatedevice) - Update Device

## comCrmDeviceSelfServiceResourceGetContactDevices

Get a list of devices

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_getContactDevices" method="get" path="/self-service/v2/contacts/{id}/devices" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceGetContactDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
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
import { contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-get-contact-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_getContactDevices" method="get" path="/self-service/v2/contacts/{id}/devices" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceGetContactDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
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
import { contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-get-contact-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_getContactDevices" method="get" path="/self-service/v2/contacts/{id}/devices" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceGetContactDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
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
import { contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-get-contact-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_getContactDevices" method="get" path="/self-service/v2/contacts/{id}/devices" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceGetContactDevices({
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
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
import { contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-get-contact-devices.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices(crm, {
    id: "da25d2f1-2ec4-23ec-b6e4-0a3c78721923",
    customFields: "key;value;key;value",
    electronicId: "I243WER",
    includeCharacteristics: true,
    includeSubscription: true,
    searchValue: "STB809403222",
    serialNumber: "serial001",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesRequest](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-request.md)              | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmDeviceSelfServiceResourceGetContactDevicesResponse](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmDeviceSelfServiceResourceAddContactDevice

Register a new device to a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_addContactDevice" method="post" path="/self-service/v2/contacts/{id}/devices" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceAddContactDevice({
    id: "<id>",
    body: {
      macAddress: "00-D0-56-F2-B5-12",
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
import { contactDevicesComCrmDeviceSelfServiceResourceAddContactDevice } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-add-contact-device.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceAddContactDevice(crm, {
    id: "<id>",
    body: {
      macAddress: "00-D0-56-F2-B5-12",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceAddContactDevice failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmDeviceSelfServiceResourceAddContactDeviceRequest](../../models/operations/com-crm-device-self-service-resource-add-contact-device-request.md)                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmDeviceSelfServiceResourceAddContactDeviceResponse](../../models/operations/com-crm-device-self-service-resource-add-contact-device-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmDeviceSelfServiceResourceListDeviceMeterReadings

Retrieve detailed information for a device's meter readings

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_listDeviceMeterReadings" method="get" path="/self-service/v2/contacts/{id}/devices/{dev_id}/meter_readings" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceListDeviceMeterReadings({
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
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
import { contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-list-device-meter-readings.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings(crm, {
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_listDeviceMeterReadings" method="get" path="/self-service/v2/contacts/{id}/devices/{dev_id}/meter_readings" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceListDeviceMeterReadings({
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
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
import { contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-list-device-meter-readings.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings(crm, {
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_listDeviceMeterReadings" method="get" path="/self-service/v2/contacts/{id}/devices/{dev_id}/meter_readings" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceListDeviceMeterReadings({
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
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
import { contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-list-device-meter-readings.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings(crm, {
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_listDeviceMeterReadings" method="get" path="/self-service/v2/contacts/{id}/devices/{dev_id}/meter_readings" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceListDeviceMeterReadings({
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
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
import { contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-list-device-meter-readings.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings(crm, {
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_listDeviceMeterReadings" method="get" path="/self-service/v2/contacts/{id}/devices/{dev_id}/meter_readings" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceListDeviceMeterReadings({
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
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
import { contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-list-device-meter-readings.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings(crm, {
    devId: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    id: "c39c6c23-319f-ef74-37cd-9b7878992fc1",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsRequest](../../models/operations/com-crm-device-self-service-resource-list-device-meter-readings-request.md) | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsResponse](../../models/operations/com-crm-device-self-service-resource-list-device-meter-readings-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmDeviceSelfServiceResourceCreateDeviceMeterReading

Create a new meter reading for a device.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_createDeviceMeterReading" method="post" path="/self-service/v2/contacts/{id}/devices/{dev_id}/meter_readings" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceCreateDeviceMeterReading({
    devId: "0b8e03c1-01e4-9c44-533a-d55b9ab0821e",
    id: "0b8e03c1-01e4-9c44-533a-d55b9ab0821e",
    body: {
      reading: 1.09,
      dates: {
        from: 1683547447,
        to: 1683547447,
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
import { contactDevicesComCrmDeviceSelfServiceResourceCreateDeviceMeterReading } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-create-device-meter-reading.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceCreateDeviceMeterReading(crm, {
    devId: "0b8e03c1-01e4-9c44-533a-d55b9ab0821e",
    id: "0b8e03c1-01e4-9c44-533a-d55b9ab0821e",
    body: {
      reading: 1.09,
      dates: {
        from: 1683547447,
        to: 1683547447,
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceCreateDeviceMeterReading failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                        | Type                                                                                                                                                                             | Required                                                                                                                                                                         | Description                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                        | [operations.ComCrmDeviceSelfServiceResourceCreateDeviceMeterReadingRequest](../../models/operations/com-crm-device-self-service-resource-create-device-meter-reading-request.md) | :heavy_check_mark:                                                                                                                                                               | The request object to use for the request.                                                                                                                                       |
| `options`                                                                                                                                                                        | RequestOptions                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                               | Used to set various options for making HTTP requests.                                                                                                                            |
| `options.fetchOptions`                                                                                                                                                           | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                          | :heavy_minus_sign:                                                                                                                                                               | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.   |
| `options.retries`                                                                                                                                                                | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                               | Enables retrying HTTP requests under certain failure conditions.                                                                                                                 |

### Response

**Promise\<[operations.ComCrmDeviceSelfServiceResourceCreateDeviceMeterReadingResponse](../../models/operations/com-crm-device-self-service-resource-create-device-meter-reading-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmDeviceSelfServiceResourceRemoveContactDevice

Delete an existing contact device

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_removeContactDevice" method="delete" path="/self-service/v2/contacts/{id}/devices/{fcm_token}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactDevices.comCrmDeviceSelfServiceResourceRemoveContactDevice({
    fcmToken: "<value>",
    id: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactDevicesComCrmDeviceSelfServiceResourceRemoveContactDevice } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-remove-contact-device.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceRemoveContactDevice(crm, {
    fcmToken: "<value>",
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceRemoveContactDevice failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmDeviceSelfServiceResourceRemoveContactDeviceRequest](../../models/operations/com-crm-device-self-service-resource-remove-contact-device-request.md)          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmDeviceSelfServiceResourceUpdateDevice

Update a single device. A device can be updated at any point of time, but only a subset of its attributes can be updated.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.DeviceSelfServiceResource_updateDevice" method="put" path="/self-service/v2/devices/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactDevices.comCrmDeviceSelfServiceResourceUpdateDevice({
    id: "0b8e03c1-01e4-9c44-533a-d55b9ab0821e",
    body: {
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
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
import { contactDevicesComCrmDeviceSelfServiceResourceUpdateDevice } from "crm/funcs/contact-devices-com-crm-device-self-service-resource-update-device.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactDevicesComCrmDeviceSelfServiceResourceUpdateDevice(crm, {
    id: "0b8e03c1-01e4-9c44-533a-d55b9ab0821e",
    body: {
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactDevicesComCrmDeviceSelfServiceResourceUpdateDevice failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmDeviceSelfServiceResourceUpdateDeviceRequest](../../models/operations/com-crm-device-self-service-resource-update-device-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmDeviceSelfServiceResourceUpdateDeviceResponse](../../models/operations/com-crm-device-self-service-resource-update-device-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |