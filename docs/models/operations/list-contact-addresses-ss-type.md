# ListContactAddressesSSType

The address type. There can be multiple addresses of the same type.

## Example Usage

```typescript
import { ListContactAddressesSSType } from "crm/models/operations";

let value: ListContactAddressesSSType = "HOME";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"HOME" | "BUSINESS" | "ALTERNATIVE" | Unrecognized<string>
```