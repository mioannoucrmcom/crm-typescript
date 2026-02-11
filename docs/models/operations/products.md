# Products

Products that should be included in the basket for the Promotion to be applied. Product conditions are defined as groups of conditions. In Each group there’s a product setting and the conditions that should be met. Multiple groups can be added, logically separated by AND/OR operators.

## Example Usage

```typescript
import { Products } from "crmcom/models/operations";

let value: Products = {
  groups: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                  | Type                                                   | Required                                               | Description                                            |
| ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ |
| `groups`                                               | [operations.Group](../../models/operations/group.md)[] | :heavy_minus_sign:                                     | Groups of product conditions.                          |