# ComCrmProductSelfServiceResourceGetProductMandatoryProduct

The mandatory product. Optional and applicable only for flexible bundle products and only if the composition refers to a “COMPONENT_SET”. Only FLAT products can be specified. Once specified, then on ordering the flexible bundle, the specified mandatory product is automatically included in the flex bundle to order.

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductMandatoryProduct } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductMandatoryProduct = {
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