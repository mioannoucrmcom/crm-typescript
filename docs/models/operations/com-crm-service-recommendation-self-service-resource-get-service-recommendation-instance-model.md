# ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationInstanceModel

Determines whether a service is managed as a single quantity or as separate, independently managed instances on a subscription

## Example Usage

```typescript
import {
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationInstanceModel,
} from "crm/models/operations";

let value:
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationInstanceModel =
    "QUANTITY_BASED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"QUANTITY_BASED" | "LINE_BASED" | Unrecognized<string>
```