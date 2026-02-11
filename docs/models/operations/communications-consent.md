# CommunicationsConsent

Messages of consent to receive marketing material

## Example Usage

```typescript
import { CommunicationsConsent } from "crm/models/operations";

let value: CommunicationsConsent = {
  emailConsent:
    "Yes, I wish to receive details about offers and promotions via email",
  smsConsent:
    "Yes, I wish to receive details about offers and promotions via SMS",
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          | Example                                                              |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `emailConsent`                                                       | *string*                                                             | :heavy_minus_sign:                                                   | Email consent message                                                | Yes, I wish to receive details about offers and promotions via email |
| `smsConsent`                                                         | *string*                                                             | :heavy_minus_sign:                                                   | SMS consent message                                                  | Yes, I wish to receive details about offers and promotions via SMS   |