# ComCrmPaymentFormSelfServiceResourceGeneratePaymentFormType

The type will be utilised by CRM.COM for back-end processes. Payment forms can be used to either make a Payment or perform a Top-up. Use the “type” to differentiate the purpose of loading the payment form. 

## Example Usage

```typescript
import { ComCrmPaymentFormSelfServiceResourceGeneratePaymentFormType } from "crm/models/operations";

let value: ComCrmPaymentFormSelfServiceResourceGeneratePaymentFormType =
  "TOP_UP";
```

## Values

```typescript
"TOP_UP" | "PAYMENT"
```