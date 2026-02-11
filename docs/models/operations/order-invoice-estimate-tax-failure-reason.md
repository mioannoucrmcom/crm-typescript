# OrderInvoiceEstimateTaxFailureReason

Shows the reason for failing to calculating taxes for the invoice, typically because there's an issue with the online taxation service

## Example Usage

```typescript
import { OrderInvoiceEstimateTaxFailureReason } from "crm/models/operations";

let value: OrderInvoiceEstimateTaxFailureReason = "INVALID_ADDRESS";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"INVALID_ADDRESS" | "API_ERROR" | "COMMUNICATION_ERROR" | Unrecognized<string>
```