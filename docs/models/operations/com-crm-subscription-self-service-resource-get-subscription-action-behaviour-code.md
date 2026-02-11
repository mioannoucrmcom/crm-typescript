# ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionBehaviourCode

The action's behaviour code shows how the action affetcs the service for example adds a new service, cancels or changes

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionBehaviourCode } from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionBehaviourCode =
    "ACTIVATE_SERVICE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BECOME_SUBSCRIBER" | "CHANGE_SUBSCRIPTION" | "TERMINATE" | "PAUSE" | "RESUME" | "ACTIVATE" | "DEACTIVATE" | "APPLY_GRACE_PERIOD" | "ADD_DEVICE" | "CHANGE_DEVICE" | "ADD_SERVICE" | "REMOVE_SERVICE" | "CHANGE_SERVICE" | "PAUSE_SERVICE" | "RESUME_SERVICE" | "CHANGE_TERMS" | "ACTIVATE_SERVICE" | "DEACTIVATE_SERVICE" | "CHANGE_SERVICE_DISTRIBUTION" | "EXTEND_SERVICE_TRIAL" | "END_GRACE_PERIOD" | Unrecognized<string>
```