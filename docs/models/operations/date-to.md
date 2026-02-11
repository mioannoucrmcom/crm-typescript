# DateTo

Filter based on the submitted 'to' date, which may fall within a given date range. The value can be a string with a date in epoch format. Each option must also include an operator. Use up to two options based on the required search (e.g. date_to[gte]=1618395497&date_to[lt]=1618395497).

## Example Usage

```typescript
import { DateTo } from "crmcom/models/operations";

let value: DateTo = "date_to[gt]";
```

## Values

```typescript
"date_to[lt]" | "date_to[lte]" | "date_to[gt]" | "date_to[gte]"
```