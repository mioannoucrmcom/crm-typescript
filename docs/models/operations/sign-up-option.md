# SignUpOption

Defines how contacts can sign up to the reward scheme

## Example Usage

```typescript
import { SignUpOption } from "crm/models/operations";

let value: SignUpOption = "SELF_SIGN_UP";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"AUTO_SIGN_UP" | "SELF_SIGN_UP" | "CLOSE_LOOP_SIGN_UP" | Unrecognized<string>
```