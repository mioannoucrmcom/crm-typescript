<!-- Start SDK Example Usage [usage] -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactAccounts
    .comCrmAccountSelfServiceResourceGetSingle({
      id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    });

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->