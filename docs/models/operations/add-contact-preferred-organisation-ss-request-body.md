# AddContactPreferredOrganisationSSRequestBody

## Example Usage

```typescript
import { AddContactPreferredOrganisationSSRequestBody } from "crmcom/models/operations";

let value: AddContactPreferredOrganisationSSRequestBody = {
  organisationId: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
  type: "ORDERS",
};
```

## Fields

| Field                                                                                                                     | Type                                                                                                                      | Required                                                                                                                  | Description                                                                                                               | Example                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `organisationId`                                                                                                          | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | The organisation identifier                                                                                               | 1a6a85ac-aacf-4175-8de2-a7d701186d96                                                                                      |
| `type`                                                                                                                    | [operations.AddContactPreferredOrganisationSSType](../../models/operations/add-contact-preferred-organisation-ss-type.md) | :heavy_check_mark:                                                                                                        | The preferred type                                                                                                        |                                                                                                                           |