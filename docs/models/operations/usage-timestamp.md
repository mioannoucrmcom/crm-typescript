# UsageTimestamp

Filter based on the usage date, which may fall within a given date range. The value can be a string with a date in epoch format. Each option must also include an operator. Use up to two options based on the required search 

## Example Usage

```typescript
import { UsageTimestamp } from "crm/models/operations";

let value: UsageTimestamp = "usage_timestamp[lte]";
```

## Values

```typescript
"usage_timestamp[lt]" | "usage_timestamp[lte]" | "usage_timestamp[gt]" | "usage_timestamp[gte]"
```