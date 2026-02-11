# InvoiceEstimateType

Type of discount applied

## Example Usage

```typescript
import { InvoiceEstimateType } from "crm/models/operations";

let value: InvoiceEstimateType = "AD_HOC";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AD_HOC" | "PROMOTION" | "AUTO_APPLIED" | Unrecognized<string>
```