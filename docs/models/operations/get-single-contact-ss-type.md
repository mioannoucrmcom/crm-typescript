# GetSingleContactSSType

Contact type - can be PERSON or COMPANY

## Example Usage

```typescript
import { GetSingleContactSSType } from "crmcom/models/operations";

let value: GetSingleContactSSType = "COMPANY";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PERSON" | "COMPANY" | Unrecognized<string>
```