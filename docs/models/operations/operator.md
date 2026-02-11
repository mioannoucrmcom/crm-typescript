# Operator

Logical operator used amount the product conditions

## Example Usage

```typescript
import { Operator } from "crm/models/operations";

let value: Operator = "AND";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AND" | "OR" | Unrecognized<string>
```