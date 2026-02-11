# CrossSellTiers

Available only Tiered, Volume and Stairstep pricing models. Only the first tier range is returned that has the returned price

## Example Usage

```typescript
import { CrossSellTiers } from "crm/models/operations";

let value: CrossSellTiers = {
  upperTier: 1,
  numberOfTiers: 3,
};
```

## Fields

| Field                                    | Type                                     | Required                                 | Description                              | Example                                  |
| ---------------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| `upperTier`                              | *number*                                 | :heavy_minus_sign:                       | The upper tier of the first tiered range | 1                                        |
| `numberOfTiers`                          | *number*                                 | :heavy_minus_sign:                       | Tiered price lower tier                  | 3                                        |