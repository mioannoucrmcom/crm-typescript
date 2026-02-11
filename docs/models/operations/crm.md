# Crm

Defines the supported crm features

## Example Usage

```typescript
import { Crm } from "crm/models/operations";

let value: Crm = {
  isSupported: true,
  serviceRequests: {
    isSupported: true,
  },
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               | Example                                                                   |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `isSupported`                                                             | *boolean*                                                                 | :heavy_minus_sign:                                                        | Defines whether contact features should be available                      | true                                                                      |
| `serviceRequests`                                                         | [operations.ServiceRequests](../../models/operations/service-requests.md) | :heavy_minus_sign:                                                        | Defines the supported service request features                            |                                                                           |