# CrmComPrintoutSelfServiceResourceOutputRequest

## Example Usage

```typescript
import { CrmComPrintoutSelfServiceResourceOutputRequest } from "crm/models/operations";

let value: CrmComPrintoutSelfServiceResourceOutputRequest = {
  entity: {
    type: "INVOICE",
    id: "007c08166f95-8c54d563-b991-4b76-8a83",
  },
  format: "PDF",
};
```

## Fields

| Field                                                                                                                                                                          | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    | Example                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `entity`                                                                                                                                                                       | [operations.CrmComPrintoutSelfServiceResourceOutputEntity](../../models/operations/crm-com-printout-self-service-resource-output-entity.md)                                    | :heavy_check_mark:                                                                                                                                                             | Defines the entity based on which the printout will be created                                                                                                                 |                                                                                                                                                                                |
| `format`                                                                                                                                                                       | [operations.CrmComPrintoutSelfServiceResourceOutputFormat](../../models/operations/crm-com-printout-self-service-resource-output-format.md)                                    | :heavy_check_mark:                                                                                                                                                             | Defines the format on which the printout will be created to<br/><br/>    EMAIL - Printout will be sent to the contact’s email address<br/>    PDF - Printout will be generated as pdf<br/> | PDF                                                                                                                                                                            |