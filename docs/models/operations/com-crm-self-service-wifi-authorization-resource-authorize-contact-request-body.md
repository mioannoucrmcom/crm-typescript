# ComCrmSelfServiceWifiAuthorizationResourceAuthorizeContactRequestBody

## Example Usage

```typescript
import { ComCrmSelfServiceWifiAuthorizationResourceAuthorizeContactRequestBody } from "crm/models/operations";

let value:
  ComCrmSelfServiceWifiAuthorizationResourceAuthorizeContactRequestBody = {
    macAddress: "01-23-45-67-89-AB",
    estimationId: "0ba7de75-8a68-c19a-3d3a-f4708723a1a4",
    siteId: "onwuq8y1",
  };
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   | Example                                                                       |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `macAddress`                                                                  | *string*                                                                      | :heavy_check_mark:                                                            | The contat’s device MAC address                                               | 01-23-45-67-89-AB                                                             |
| `estimationId`                                                                | *string*                                                                      | :heavy_check_mark:                                                            | The usage estimation (identifier) that the contact is authorized for          | 0ba7de75-8a68-c19a-3d3a-f4708723a1a4                                          |
| `siteId`                                                                      | *string*                                                                      | :heavy_check_mark:                                                            | The site (organisation’s WiFi network) that the contact is authorized against | onwuq8y1                                                                      |