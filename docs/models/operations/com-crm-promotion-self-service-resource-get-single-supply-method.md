# ComCrmPromotionSelfServiceResourceGetSingleSupplyMethod

The type of the event:
 * `DELIVERY` - Delivered to the customer’s address
 * `PICK_UP` - Picked up by the customer from a venue
 * `DIRECT_SALE` - Online sales of services


## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceGetSingleSupplyMethod } from "crm/models/operations";

let value: ComCrmPromotionSelfServiceResourceGetSingleSupplyMethod = "DELIVERY";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DELIVERY" | "PICK_UP" | "DIRECT_SALE" | Unrecognized<string>
```