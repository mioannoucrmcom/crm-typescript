# ComCrmPassPlanSelfServiceResourceListPassTypesProduct

The product related to the Pass Plan. Applicable only for Electronic Gift pass plans, but optional. If specified, then electronic gift passes will be available for contacts to be purchased in a front-end system. Only flat, non-traceable physical goods can be specified.

## Example Usage

```typescript
import { ComCrmPassPlanSelfServiceResourceListPassTypesProduct } from "crmcom/models/operations";

let value: ComCrmPassPlanSelfServiceResourceListPassTypesProduct = {
  id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
  name: "Universal Name",
  sku: "S0001",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | e283a863-18e1-7cae-48c4-7433bf28cf97 |
| `name`                               | *string*                             | :heavy_minus_sign:                   | The entity name                      | Universal Name                       |
| `sku`                                | *string*                             | :heavy_minus_sign:                   | The entity sku                       | S0001                                |