# OrderUnavailabilityReason

Details on why the product is considered as invalid and cannot be included in the Order
 * `VALIDITY_PERIOD` - The prodcut’s validity period has expired, i.e. the business is no longer selling this product
 * `AVAILABILITY` - The product is temporarily un-available for sale at/by the requested organisation e.g. is out of stock
 * `ORDER_CATALOGUE` - The product is not included in an valid/effective Order Catalogue.
 * `STOCK` - The product does not have enough stock.


## Example Usage

```typescript
import { OrderUnavailabilityReason } from "crmcom/models/operations";

let value: OrderUnavailabilityReason = "STOCK";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"STOCK" | "VALIDITY_PERIOD" | "AVAILABILITY" | "ORDER_CATALOGUE" | Unrecognized<string>
```