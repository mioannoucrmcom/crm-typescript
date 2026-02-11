# ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationProductTaxModel

Defines whether the price is tax inclusive or not. Defaults to the system's Taxation setting

## Example Usage

```typescript
import {
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationProductTaxModel,
} from "crmcom/models/operations";

let value:
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationProductTaxModel =
    "TAX_INCLUSIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"TAX_INCLUSIVE" | "TAX_EXCLUSIVE" | Unrecognized<string>
```