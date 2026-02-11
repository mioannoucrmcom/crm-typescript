# Sort

Defines on which attribute the results should be sorted by, can be DEFAULT_SORTING, ORGANISATION_NAME, DISTANCE (lat & lon must be specified too)

## Example Usage

```typescript
import { Sort } from "crm/models/operations";

let value: Sort = "ORGANISATION_NAME";
```

## Values

```typescript
"DEFAULT_SORTING" | "ORGANISATION_NAME" | "DISTANCE"
```