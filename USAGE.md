<!-- Start SDK Example Usage [usage] -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAccounts
    .comCrmAccountSelfServiceResourceGetSingle({
      id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    });

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->