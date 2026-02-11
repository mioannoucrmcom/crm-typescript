# ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsResponse

OK

## Example Usage

```typescript
import { ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsResponse } from "crm/models/operations";

let value: ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsResponse =
  {
    content: [
      {
        name: "Reset PIN",
        description: "Resets the PIN to a given value",
        metadataAttributes: [
          {
            key: "pin",
            label: "PIN",
            description: "The new pin",
            isMandatory: true,
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                    | Type                                                                                                                                                                                     | Required                                                                                                                                                                                 | Description                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `content`                                                                                                                                                                                | [operations.ComCrmServiceCommandsSelfServiceResourceGetServiceCommandsContent](../../models/operations/com-crm-service-commands-self-service-resource-get-service-commands-content.md)[] | :heavy_minus_sign:                                                                                                                                                                       | N/A                                                                                                                                                                                      |