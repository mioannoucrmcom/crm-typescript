# ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionTaxFailureReason

Shows the reason for failing to calculating taxes for the invoice, typically because there's an issue with the online taxation service

## Example Usage

```typescript
import {
  ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionTaxFailureReason,
} from "crm/models/operations";

let value:
  ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionTaxFailureReason =
    "INVALID_ADDRESS";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"INVALID_ADDRESS" | "API_ERROR" | "COMMUNICATION_ERROR" | Unrecognized<string>
```