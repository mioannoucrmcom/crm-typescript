# ProductType

The awarded product type

## Example Usage

```typescript
import { ProductType } from "crmcom/models/operations";

let value: ProductType = "TYPE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SKU" | "BRAND" | "TYPE" | "FAMILY" | Unrecognized<string>
```