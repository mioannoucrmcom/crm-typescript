# SignUpOption

Defines how contacts can sign up to the reward scheme

## Example Usage

```typescript
import { SignUpOption } from "crmcom/models/operations";

let value: SignUpOption = "SELF_SIGN_UP";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AUTO_SIGN_UP" | "SELF_SIGN_UP" | "CLOSE_LOOP_SIGN_UP" | Unrecognized<string>
```