# ComCrmOrderSelfServiceResourceGetOrderBundledItem

Applicable when the ordered items is bundled with another order item. The bundled item is a fixed/flexible bundle or a Composite product. Each componnet/modifier selected during the ordering flow is retured as an individual order item so the bunlded item can be used to identify which components/modifiered wasere actually ordered.

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceGetOrderBundledItem } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceGetOrderBundledItem = {};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                 | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The bundled order item's identifier                                                                                                                                  |
| `product`                                                                                                                                                            | [operations.ComCrmOrderSelfServiceResourceGetOrderBundledItemProduct](../../models/operations/com-crm-order-self-service-resource-get-order-bundled-item-product.md) | :heavy_minus_sign:                                                                                                                                                   | The bundle product                                                                                                                                                   |