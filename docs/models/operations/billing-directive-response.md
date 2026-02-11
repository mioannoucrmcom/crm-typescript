# BillingDirectiveResponse

The usage record's billing directive shows if the usage will be billed or not

## Example Usage

```typescript
import { BillingDirectiveResponse } from "crm/models/operations";

let value: BillingDirectiveResponse = "TO_BE_BILLED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"TO_BE_BILLED" | "TO_BE_CREDITED" | "NOT_TO_BE_BILLED" | Unrecognized<string>
```