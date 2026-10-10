# ComCrmContactSelfServiceResourceListContactRelationshipState

The community member’s relation state. A person is considered as a valid community person only after they accept the invitation to join the community.

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceListContactRelationshipState } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceListContactRelationshipState =
  "ACCEPTED";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"PENDING" | "ACCEPTED" | "REJECTED" | Unrecognized<string>
```