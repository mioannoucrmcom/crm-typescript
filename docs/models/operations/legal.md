# Legal

Legal configuration for Landing Pages of type 'REGISTER'

## Example Usage

```typescript
import { Legal } from "crm/models/operations";

let value: Legal = {
  termsOfService: {
    acceptanceMessage: "I accept the #terms_conditions and #privacy_policy",
    termsConditions:
      "1) Acceptance of Terms: By using this app, you agree to abide by the terms and conditions outlined herein. 2) Intellectual Property: The app and its contents are protected by intellectual property rights. You may not use, copy, or distribute any materials from the app without prior written permission...",
    privacyPolicy:
      "Close Cut Hair Salon is committed to protecting and using personal information which is collected or will be collected appropriately...",
    termsConditionsLink:
      "1) Acceptance of Terms: By using this app, you agree to abide by the terms and conditions outlined herein. 2) Intellectual Property: The app and its contents are protected by intellectual property rights. You may not use, copy, or distribute any materials from the app without prior written permission...",
    privacyPolicyLink:
      "Close Cut Hair Salon is committed to protecting and using personal information which is collected or will be collected appropriately...",
  },
  communicationsConsent: {
    emailConsent:
      "Yes, I wish to receive details about offers and promotions via email",
    smsConsent:
      "Yes, I wish to receive details about offers and promotions via SMS",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `termsOfService`                                                                      | [operations.TermsOfService](../../models/operations/terms-of-service.md)              | :heavy_minus_sign:                                                                    | Details of terms & conditions and privacy policy                                      |
| `communicationsConsent`                                                               | [operations.CommunicationsConsent](../../models/operations/communications-consent.md) | :heavy_minus_sign:                                                                    | Messages of consent to receive marketing material                                     |