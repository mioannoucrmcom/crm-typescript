# ComCrmApplicationSelfServiceResourceListDetails

Required details per supported payment method

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceListDetails } from "crmcom/models/operations";

let value: ComCrmApplicationSelfServiceResourceListDetails = {};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `accountDebit`                                                                                      | *string*[]                                                                                          | :heavy_minus_sign:                                                                                  | The bank details.Required and applicable if the payment method is set to Account Debit such as SEPA |