# ComCrmAccountSelfServiceResourceGetAccountJournalRequest

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceGetAccountJournalRequest } from "crm/models/operations";

let value: ComCrmAccountSelfServiceResourceGetAccountJournalRequest = {
  id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
  includeLines: false,
};
```

## Fields

| Field                                           | Type                                            | Required                                        | Description                                     | Example                                         |
| ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| `id`                                            | *string*                                        | :heavy_check_mark:                              | The journal id to retrieve information for      | CAD1E31269B76D7A65ACCE45B2E68DFD                |
| `includeLines`                                  | *boolean*                                       | :heavy_minus_sign:                              | Include financial transation lines in response? | false                                           |