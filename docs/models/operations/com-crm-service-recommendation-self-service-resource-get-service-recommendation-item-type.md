# ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationItemType

Allowed components can be individual products or products of a specific type, family, component set or category

## Example Usage

```typescript
import { ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationItemType } from "crm/models/operations";

let value:
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationItemType =
    "PRODUCT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PRODUCT" | "FAMILY" | "TYPE" | "CATEGORY" | "COMPONENT_SET" | Unrecognized<string>
```