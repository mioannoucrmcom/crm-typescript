# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesInstanceModel

Determines whether a service is managed as a single quantity or as separate, independently managed instances on subscription

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesInstanceModel } from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesInstanceModel =
    "QUANTITY_BASED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"QUANTITY_BASED" | "LINE_BASED" | Unrecognized<string>
```