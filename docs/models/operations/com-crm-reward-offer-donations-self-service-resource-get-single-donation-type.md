# ComCrmRewardOfferDonationsSelfServiceResourceGetSingleDonationType

Defines how the donated amount will be calculated on each donation made by the contact. In Spare Change and Fixed types, the business defines the donated amount’s rules, whereas in Variable type, the contact decides how much to donate.

## Example Usage

```typescript
import { ComCrmRewardOfferDonationsSelfServiceResourceGetSingleDonationType } from "crm/models/operations";

let value: ComCrmRewardOfferDonationsSelfServiceResourceGetSingleDonationType =
  "TERMED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PER_TRANSACTION" | "TERMED" | "VARIABLE" | Unrecognized<string>
```