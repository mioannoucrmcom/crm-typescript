# ComCrmRewardOfferDonationsSelfServiceResourceListDonationType

Defines how the donated amount will be calculated on each donation made by the contact. In Spare Change and Fixed types, the business defines the donated amount’s rules, whereas in Variable type, the contact decides how much to donate.

## Example Usage

```typescript
import { ComCrmRewardOfferDonationsSelfServiceResourceListDonationType } from "crm/models/operations";

let value: ComCrmRewardOfferDonationsSelfServiceResourceListDonationType =
  "VARIABLE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"PER_TRANSACTION" | "TERMED" | "VARIABLE" | Unrecognized<string>
```