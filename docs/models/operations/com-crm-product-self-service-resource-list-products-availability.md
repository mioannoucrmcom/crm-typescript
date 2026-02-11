# ComCrmProductSelfServiceResourceListProductsAvailability

Denotes whether the product is available for ordering at the organisation that will fulfill the order. Available only if a fulfilled by organisation is set in the method's filters

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceListProductsAvailability } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceListProductsAvailability = "ENABLED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ENABLED" | "DISABLED" | Unrecognized<string>
```