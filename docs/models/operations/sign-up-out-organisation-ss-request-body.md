# SignUpOutOrganisationSSRequestBody

## Example Usage

```typescript
import { SignUpOutOrganisationSSRequestBody } from "crm/models/operations";

let value: SignUpOutOrganisationSSRequestBody = {
  action: "SIGNUP",
  organisationId: "9086dd6b-2b9f-4fba-85ff-1b89143a56da",
  emailOptOut: true,
  smsOptOut: true,
  referralCode: "IX4B0M",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               | Example                                                                                                   |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `action`                                                                                                  | [operations.SignUpOutOrganisationSSAction](../../models/operations/sign-up-out-organisation-ss-action.md) | :heavy_check_mark:                                                                                        | The action to be taken                                                                                    | SIGNUP                                                                                                    |
| `organisationId`                                                                                          | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The organisation identifier on which the action will be applied                                           | 9086dd6b-2b9f-4fba-85ff-1b89143a56da                                                                      |
| `serviceAcceptance`                                                                                       | *boolean*                                                                                                 | :heavy_minus_sign:                                                                                        | Defines whether the contact has accepted the client service (applicable only if action is SIGNUP)         | true                                                                                                      |
| `emailOptOut`                                                                                             | *boolean*                                                                                                 | :heavy_minus_sign:                                                                                        | The contact setting for receiving emails (applicable only if action is SIGNUP)                            | true                                                                                                      |
| `smsOptOut`                                                                                               | *boolean*                                                                                                 | :heavy_minus_sign:                                                                                        | The contact setting for receiving sms (applicable only if action is SIGNUP)                               | true                                                                                                      |
| `referralCode`                                                                                            | *string*                                                                                                  | :heavy_minus_sign:                                                                                        | The code that will be used for awarding referral events (applicable only if action is SIGNUP)             | IX4B0M                                                                                                    |