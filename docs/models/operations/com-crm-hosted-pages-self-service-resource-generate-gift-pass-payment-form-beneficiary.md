# ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormBeneficiary

Details about the beneficiary

## Example Usage

```typescript
import { ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormBeneficiary } from "crm/models/operations";

let value:
  ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormBeneficiary = {
    name: "<value>",
    email: "Chaim_Breitenberg5@yahoo.com",
    language: "EN",
  };
```

## Fields

| Field                                                                                                                                                        | Type                                                                                                                                                         | Required                                                                                                                                                     | Description                                                                                                                                                  | Example                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `name`                                                                                                                                                       | *string*                                                                                                                                                     | :heavy_check_mark:                                                                                                                                           | The name of the beneficiary                                                                                                                                  |                                                                                                                                                              |
| `email`                                                                                                                                                      | *string*                                                                                                                                                     | :heavy_check_mark:                                                                                                                                           | The email address of the beneficiary                                                                                                                         |                                                                                                                                                              |
| `language`                                                                                                                                                   | *string*                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                           | The 2-character language code in which the communication will be sent to the recipient. If not provided, the default language of the automation will be used | EN                                                                                                                                                           |