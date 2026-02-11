# InvoiceEstimateProductClassification

The product’s classification

## Example Usage

```typescript
import { InvoiceEstimateProductClassification } from "crmcom/models/operations";

let value: InvoiceEstimateProductClassification = "TRACEABLE_PHYSICAL_GOOD";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"TERMED_SERVICE" | "USAGE_SERVICE" | "ONE_TIME_SERVICE" | "TRACEABLE_PHYSICAL_GOOD" | "NON_TRACEABLE_PHYSICAL_GOOD" | "EXPENSES_SERVICE" | Unrecognized<string>
```