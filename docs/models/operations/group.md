# Group

## Example Usage

```typescript
import { Group } from "crmcom/models/operations";

let value: Group = {
  group: "G1",
  operator: "AND",
  conditions: [
    {
      operator: "OR",
      product: {
        itemType: "SKU",
        itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        sku: "HDSTB123",
        name: "HD STB",
      },
      quantity: 1,
      value: 9.99,
      billingCycle: {
        duration: 1,
        uot: "DAY",
      },
      contractPeriod: {
        duration: 12,
        uot: "MONTH",
      },
      services: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          sku: "TV001",
          name: "Films",
          quantity: 2,
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                           | Type                                                                                                                                                            | Required                                                                                                                                                        | Description                                                                                                                                                     | Example                                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `group`                                                                                                                                                         | *string*                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                              | The group’s name. Each group name must be unique                                                                                                                | G1                                                                                                                                                              |
| `operator`                                                                                                                                                      | [operations.Operator](../../models/operations/operator.md)                                                                                                      | :heavy_minus_sign:                                                                                                                                              | Logical operator used amount the product conditions                                                                                                             | AND                                                                                                                                                             |
| `conditions`                                                                                                                                                    | [operations.Condition](../../models/operations/condition.md)[]                                                                                                  | :heavy_minus_sign:                                                                                                                                              | List of product conditions. Mulitple conditions can be added, each one referring to a single product. All product conditions must be met to apply the promotion |                                                                                                                                                                 |