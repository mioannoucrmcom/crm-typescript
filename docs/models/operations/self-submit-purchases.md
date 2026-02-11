# SelfSubmitPurchases

Defines the supported contact self-submit purchase events features

## Example Usage

```typescript
import { SelfSubmitPurchases } from "crmcom/models/operations";

let value: SelfSubmitPurchases = {
  isSupported: true,
  selfSubmitMethods: [
    "BARCODE",
  ],
};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      | Example                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `isSupported`                                                                                                    | *boolean*                                                                                                        | :heavy_minus_sign:                                                                                               | Defines whether contact can self-submit purchase events                                                          | true                                                                                                             |
| `selfSubmitMethods`                                                                                              | [operations.SelfSubmitMethod](../../models/operations/self-submit-method.md)[]                                   | :heavy_minus_sign:                                                                                               | Defines how reclaim purchase identification will be made (required when contact self-submit purchase is enabled) |                                                                                                                  |