# IdType

The type of the ID to be provided

## Example Usage

```typescript
import { IdType } from "crmcom/models/operations";

let value: IdType = "BRAND";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PRODUCT" | "TYPE" | "FAMILY" | "BRAND" | Unrecognized<string>
```