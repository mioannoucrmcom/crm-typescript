# ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsBusinessClassificationCode

The business classification code shows additional information about the action and its results such as service is added as draft or effective

## Example Usage

```typescript
import {
  ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsBusinessClassificationCode,
} from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsBusinessClassificationCode =
    "REMOVE_DEVICE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BECOME_SUBSCRIBER" | "CHANGE_BILLING_CYCLE" | "CHANGE_BILLING_DAY" | "CHANGE_PAYMENT_METHOD" | "PAUSE" | "RESUME" | "CANCEL" | "REGRET" | "ACTIVATE" | "DEACTIVATE" | "APPLY_GRACE_PERIOD" | "ADD_DEVICE" | "REMOVE_DEVICE" | "REPLACE_DEVICE" | "UPDATE_DEVICE" | "ADD_SERVICE_AS_EFFECTIVE" | "ADD_SERVICE_AS_DRAFT" | "CANCEL_SERVICE" | "REGRET_SERVICE" | "UPGRADE_SERVICE" | "DOWNGRADE_SERVICE" | "PAUSE_SERVICE" | "RESUME_SERVICE" | "OPT_IN_RENEWALS" | "OPT_OUT_RENEWALS" | "RENEW_TERMS" | "RENEW_CONTRACT" | "EXTEND_CONTRACT" | "ACTIVATE_SERVICE" | "DEACTIVATE_SERVICE" | "CHANGE_SERVICE_DISTRIBUTION" | "EXTEND_SERVICE_TRIAL" | Unrecognized<string>
```