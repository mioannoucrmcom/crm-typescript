# Donations

Indicates whether the donations feature is supported

## Example Usage

```typescript
import { Donations } from "crm/models/operations";

let value: Donations = {};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `isSupported`                                                                   | *boolean*                                                                       | :heavy_minus_sign:                                                              | If there is at least one valid reward offer enabled then the 'true' is returned |