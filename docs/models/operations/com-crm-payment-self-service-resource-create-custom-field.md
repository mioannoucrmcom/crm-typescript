# ComCrmPaymentSelfServiceResourceCreateCustomField

A list of custom fields whose values can be set when creating or updating entities

## Example Usage

```typescript
import { ComCrmPaymentSelfServiceResourceCreateCustomField } from "crm/models/operations";

let value: ComCrmPaymentSelfServiceResourceCreateCustomField = {
  key: "back_office",
  value: "0001-12345",
};
```

## Fields

| Field                         | Type                          | Required                      | Description                   | Example                       |
| ----------------------------- | ----------------------------- | ----------------------------- | ----------------------------- | ----------------------------- |
| `key`                         | *string*                      | :heavy_minus_sign:            | The custom field’s unique key | back_office                   |
| `value`                       | *string*                      | :heavy_minus_sign:            | The custom field’s value      | 0001-12345                    |