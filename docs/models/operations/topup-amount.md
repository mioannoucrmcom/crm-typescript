# TopupAmount

## Example Usage

```typescript
import { TopupAmount } from "crm/models/operations";

let value: TopupAmount = {
  currencyCode: "EUR",
  amounts: [
    10,
    20,
    50,
    100,
  ],
};
```

## Fields

| Field                                                                                                                                                                           | Type                                                                                                                                                                            | Required                                                                                                                                                                        | Description                                                                                                                                                                     | Example                                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `currencyCode`                                                                                                                                                                  | [operations.ComCrmApplicationSelfServiceResourceGetApplicationCurrencyCode](../../models/operations/com-crm-application-self-service-resource-get-application-currency-code.md) | :heavy_minus_sign:                                                                                                                                                              | Currency code the top up amounts, will be displayed on the Application screen                                                                                                   | EUR                                                                                                                                                                             |
| `amounts`                                                                                                                                                                       | *number*[]                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                              | The top up amount options                                                                                                                                                       | [<br/>10,<br/>20,<br/>50,<br/>100<br/>]                                                                                                                                         |