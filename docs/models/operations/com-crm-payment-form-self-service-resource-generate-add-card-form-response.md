# ComCrmPaymentFormSelfServiceResourceGenerateAddCardFormResponse

OK

## Example Usage

```typescript
import { ComCrmPaymentFormSelfServiceResourceGenerateAddCardFormResponse } from "crm/models/operations";

let value: ComCrmPaymentFormSelfServiceResourceGenerateAddCardFormResponse = {};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `formHtml`                                                                                                   | *string*                                                                                                     | :heavy_minus_sign:                                                                                           | The HTML content used to render the payment form on the front-end, and is directly displayed to the contact. |
| `formUrl`                                                                                                    | *string*                                                                                                     | :heavy_minus_sign:                                                                                           | The URL of the hosted payment form, to which the contact must be redirected.                                 |