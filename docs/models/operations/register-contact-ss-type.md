# RegisterContactSSType

Contact type - can be PERSON or COMPANY

## Example Usage

```typescript
import { RegisterContactSSType } from "crmcom/models/operations";

let value: RegisterContactSSType = "PERSON";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PERSON" | "COMPANY" | Unrecognized<string>
```