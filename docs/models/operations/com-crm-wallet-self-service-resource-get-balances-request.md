# ComCrmWalletSelfServiceResourceGetBalancesRequest

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetBalancesRequest } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetBalancesRequest = {
  id: "acf8b8ac-a325-a644-c866-a6c9d62ff11b",
  commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
  isActive: true,
};
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 | Example                                                                                                     |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                        | *string*                                                                                                    | :heavy_check_mark:                                                                                          | The unique identification of the wallet whose balance commerce pools will be retrieved.                     | acf8b8ac-a325-a644-c866-a6c9d62ff11b                                                                        |
| `commercePoolId`                                                                                            | *string*                                                                                                    | :heavy_minus_sign:                                                                                          | The id of a specific commerce pool (optional). If not provided then all commerce pools are retrieved        | 234fbc54-bc32-1990-ce59-76c45e6377a8                                                                        |
| `includeExpiration`                                                                                         | *boolean*                                                                                                   | :heavy_minus_sign:                                                                                          | If set to true, then the expiration information will also be retrieved                                      |                                                                                                             |
| `isActive`                                                                                                  | *boolean*                                                                                                   | :heavy_minus_sign:                                                                                          | If set to true, then only active commerce pools will be retrieved. By default will bring all commerce pools | true                                                                                                        |