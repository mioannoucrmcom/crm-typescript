# ComCrmOrderSelfServiceResourceListOrdersDeliveryMethod

The type of the event:
 * `DIRECT_DELIVERY` - Deliver locally by the business or the merchant
 * `COURIER_SERVICE` - Deliver by a courier service/shipping partner up
 * `PICKUP_POINT` - Deliver to a pick-up point


## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceListOrdersDeliveryMethod } from "crm/models/operations";

let value: ComCrmOrderSelfServiceResourceListOrdersDeliveryMethod =
  "PICKUP_POINT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"DIRECT_DELIVERY" | "COURIER_SERVICE" | "PICKUP_POINT" | Unrecognized<string>
```