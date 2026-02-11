# Expiration

Defines the amounts expiring in periods. Available only if the parameter include_expiration is set to true

## Example Usage

```typescript
import { Expiration } from "crmcom/models/operations";

let value: Expiration = {
  zeroToThirty: 30,
  thirtyToSixty: 50.5,
  sixtyToNinety: 55.5,
  ninetyPlus: 60,
};
```

## Fields

| Field                                            | Type                                             | Required                                         | Description                                      | Example                                          |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| `zeroToThirty`                                   | *number*                                         | :heavy_minus_sign:                               | The amount that will expire in up to 30 days     | 30                                               |
| `thirtyToSixty`                                  | *number*                                         | :heavy_minus_sign:                               | The amount that will expire from 30 to 60 days   | 50.5                                             |
| `sixtyToNinety`                                  | *number*                                         | :heavy_minus_sign:                               | The amount that will expire from 60 to 90 days   | 55.5                                             |
| `ninetyPlus`                                     | *number*                                         | :heavy_minus_sign:                               | The amount that will expire in more than 90 days | 60                                               |