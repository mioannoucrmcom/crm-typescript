# PostedOn

Filter based on the posted date, which may fall within a given date range. The value can be a string with a date in epoch format. Each option must also include an operator. Use up to two options based on the required search

## Example Usage

```typescript
import { PostedOn } from "crm/models/operations";

let value: PostedOn = "posted_on[gte]";
```

## Values

```typescript
"posted_on[lt]" | "posted_on[lte]" | "posted_on[gt]" | "posted_on[gte]"
```