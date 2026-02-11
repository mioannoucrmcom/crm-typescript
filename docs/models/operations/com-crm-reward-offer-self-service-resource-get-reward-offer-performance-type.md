# ComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformanceType

Defines the performance type of the offer, whether it’s based on transaction amount, contact events or purchased products

## Example Usage

```typescript
import { ComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformanceType } from "crmcom/models/operations";

let value: ComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformanceType =
  "AMOUNT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AMOUNT" | "PRODUCT" | "EVENT" | Unrecognized<string>
```