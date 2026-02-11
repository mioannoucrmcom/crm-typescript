# RegisterContactSSOrganisation

## Example Usage

```typescript
import { RegisterContactSSOrganisation } from "crm/models/operations";

let value: RegisterContactSSOrganisation = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  type: "ORGANISATION",
  name: "CRMdotCOM",
};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      | Example                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                             | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | The entity identifier                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                             |
| `type`                                                                                                           | [operations.RegisterContactSSOrganisationType](../../models/operations/register-contact-ss-organisation-type.md) | :heavy_minus_sign:                                                                                               | The organisation type                                                                                            | ORGANISATION                                                                                                     |
| `name`                                                                                                           | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | The organisation name                                                                                            | CRMdotCOM                                                                                                        |