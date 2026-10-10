# TrialState

Service currently in trial or not

## Example Usage

```typescript
import { TrialState } from "crm/models/operations";

let value: TrialState = "IN_TRIAL";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"IN_TRIAL" | "TRIAL_ENDED" | Unrecognized<string>
```