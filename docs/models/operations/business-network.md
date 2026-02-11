# BusinessNetwork

Defines the supported business network features

## Example Usage

```typescript
import { BusinessNetwork } from "crmcom/models/operations";

let value: BusinessNetwork = {
  isSupported: true,
  multitenancy: {
    isSupported: true,
  },
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        | Example                                                            |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `isSupported`                                                      | *boolean*                                                          | :heavy_minus_sign:                                                 | Defines whether business network features should be available      | true                                                               |
| `multitenancy`                                                     | [operations.Multitenancy](../../models/operations/multitenancy.md) | :heavy_minus_sign:                                                 | Defines whether multitenancy features will be available            |                                                                    |