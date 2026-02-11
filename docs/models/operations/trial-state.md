# TrialState

Service currently in trial or not

## Example Usage

```typescript
import { TrialState } from "crm/models/operations";

let value: TrialState = "IN_TRIAL";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"IN_TRIAL" | "TRIAL_ENDED" | Unrecognized<string>
```