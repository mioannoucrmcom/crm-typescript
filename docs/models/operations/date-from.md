# DateFrom

Filter based on the submitted 'from' date, which may fall within a given date range. The value can be a string with a date in epoch format. Each option must also include an operator. Use up to two options based on the required search (e.g. date_from[gte]=1618395497&date_from[lt]=1618395497).

## Example Usage

```typescript
import { DateFrom } from "crm/models/operations";

let value: DateFrom = "date_from[gte]";
```

## Values

```typescript
"date_from[lt]" | "date_from[lte]" | "date_from[gt]" | "date_from[gte]"
```