# ComCrmRewardSchemeSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmRewardSchemeSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmRewardSchemeSelfServiceResourceListResponse = {
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Loyalty Scheme",
      description: "Lorem Ipsum",
      signUpOption: "SELF_SIGN_UP",
      signUpMethod: "CODE",
      termsAndConditions: "Only CRMdotCOM domain customer can sign up",
      isSigned: false,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `content`                                                                                                                                            | [operations.ComCrmRewardSchemeSelfServiceResourceListContent](../../models/operations/com-crm-reward-scheme-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                   | N/A                                                                                                                                                  |