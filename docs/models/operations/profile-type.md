# ProfileType

The contact attribute

## Example Usage

```typescript
import { ProfileType } from "crmcom/models/operations";

let value: ProfileType = "NAMEDAY";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BIRTHDATE" | "NAMEDAY" | "GENDER" | Unrecognized<string>
```