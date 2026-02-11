# ComCrmContactSelfServiceResourceGetContactRelationshipItemType

Product setting. Allow usage to either a specific product or to products of a specific type or to products of a specific family or to products of a specific category

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactRelationshipItemType } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetContactRelationshipItemType =
  "PRODUCT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PRODUCT" | "TYPE" | "FAMILY" | "CATEGORY" | Unrecognized<string>
```