# crm

Developer-friendly & type-safe Typescript SDK specifically catered to leverage *crm* API.

[![Built by Speakeasy](https://img.shields.io/badge/Built_by-SPEAKEASY-374151?style=for-the-badge&labelColor=f3f4f6)](https://www.speakeasy.com/?utm_source=crm&utm_campaign=typescript)
[![License: MIT](https://img.shields.io/badge/LICENSE_//_MIT-3b5bdb?style=for-the-badge&labelColor=eff6ff)](https://opensource.org/licenses/MIT)


<br /><br />
> [!IMPORTANT]
> This SDK is not yet ready for production use. To complete setup please follow the steps outlined in your [workspace](https://app.speakeasy.com/org/marios/self-service). Delete this section before > publishing to a package manager.

<!-- Start Summary [summary] -->
## Summary

Self Service API: Self Service API
<!-- End Summary [summary] -->

<!-- Start Table of Contents [toc] -->
## Table of Contents
<!-- $toc-max-depth=2 -->
* [crm](#crm)
  * [SDK Installation](#sdk-installation)
  * [Requirements](#requirements)
  * [SDK Example Usage](#sdk-example-usage)
  * [Authentication](#authentication)
  * [Available Resources and Operations](#available-resources-and-operations)
  * [Standalone functions](#standalone-functions)
  * [File uploads](#file-uploads)
  * [Retries](#retries)
  * [Error Handling](#error-handling)
  * [Server Selection](#server-selection)
  * [Custom HTTP Client](#custom-http-client)
  * [Debugging](#debugging)
* [Development](#development)
  * [Maturity](#maturity)
  * [Contributions](#contributions)

<!-- End Table of Contents [toc] -->

<!-- Start SDK Installation [installation] -->
## SDK Installation

The SDK can be installed with either [npm](https://www.npmjs.com/), [pnpm](https://pnpm.io/), [bun](https://bun.sh/) or [yarn](https://classic.yarnpkg.com/en/) package managers.

### NPM

```bash
npm add crm
```

### PNPM

```bash
pnpm add crm
```

### Bun

```bash
bun add crm
```

### Yarn

```bash
yarn add crm
```

> [!NOTE]
> This package is published with CommonJS and ES Modules (ESM) support.
<!-- End SDK Installation [installation] -->

<!-- Start Requirements [requirements] -->
## Requirements

For supported JavaScript runtimes, please consult [RUNTIMES.md](RUNTIMES.md).
<!-- End Requirements [requirements] -->

<!-- Start SDK Example Usage [usage] -->
## SDK Example Usage

### Example

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

<!-- Start Authentication [security] -->
## Authentication

### Per-Client Security Schemes

This SDK supports the following security scheme globally:

| Name                       | Type | Scheme      | Environment Variable             |
| -------------------------- | ---- | ----------- | -------------------------------- |
| `authorizationSelfService` | http | HTTP Bearer | `CRM_AUTHORIZATION_SELF_SERVICE` |

To authenticate with the API the `authorizationSelfService` parameter must be set when initializing the SDK client instance. For example:
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

### Per-Operation Security Schemes

Some operations in this SDK require the security scheme to be specified at the request level. For example:
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.addressLookup
    .comCrmAddressRegistrySelfServiceResourceGetAddress({}, {
      googlePlaceId: "ChIJLU7jZClu5kcR4PcOOO6p3I0",
      latlng: "<value>",
      sessionId: "b9a5d80f-f2fa-4f62-b29f-9d288186bdf1",
    });

  console.log(result);
}

run();

```
<!-- End Authentication [security] -->

<!-- Start Available Resources and Operations [operations] -->
## Available Resources and Operations

<details open>
<summary>Available methods</summary>

### [AddressLookup](docs/sdks/addresslookup/README.md)

* [comCrmAddressRegistrySelfServiceResourceList](docs/sdks/addresslookup/README.md#comcrmaddressregistryselfserviceresourcelist) - Search Addresses
* [comCrmAddressRegistrySelfServiceResourceGetAddress](docs/sdks/addresslookup/README.md#comcrmaddressregistryselfserviceresourcegetaddress) - Get Address

### [ApprovalRequests](docs/sdks/approvalrequests/README.md)

* [comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourceacceptapprovalrequest) - Approve an Approval Request
* [comCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourceacceptapprovalrequestaction) - Approve an Approval Request
* [comCrmApprovalRequestSelfServiceResourceRejectApprovalRequest](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourcerejectapprovalrequest) - Show the Reject an Approval Request Form
* [comCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourcerejectapprovalrequestaction) - Reject an Approval Request
* [comCrmApprovalRequestSelfServiceResourcePerformActions](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourceperformactions) - Perform Approval Request Actions
* [comCrmApprovalRequestSelfServiceResourceList](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourcelist) - List Approval Requests

### [Authentication](docs/sdks/authentication/README.md)

* [comCrmContactSelfServiceResourceAuthenticate](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceauthenticate) - Contact Authentication
* [comCrmContactSelfServiceResourceChangeForgottenPassword](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcechangeforgottenpassword) - Change Forgotten Password
* [comCrmContactSelfServiceResourceForgotPassword](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceforgotpassword) - Forgot Password
* [comCrmContactSelfServiceResourceRequestOTP](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcerequestotp) - Request One Time Password
* [comCrmContactSelfServiceResourceRefresh](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcerefresh) - Refresh Contact Token
* [comCrmContactSelfServiceResourceEmailVerification](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceemailverification) - Request Email Verification
* [comCrmContactSelfServiceResourceValidateOTP](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcevalidateotp) - Validate One Time Password
* [comCrmContactSelfServiceResourceVerifyContactEmail](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceverifycontactemail) - Verify Contact Email
* [comCrmContactSelfServiceResourceChangePassword](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcechangepassword) - Change Password
* [addContactIdentitySS](docs/sdks/authentication/README.md#addcontactidentityss) - Add Contact Identity
* [comCrmContactSelfServiceResourceSignOut](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcesignout) - Sign Out Contact
* [comCrmContactSelfServiceResourceSwitchContact](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceswitchcontact) - Contact Switch

### [CommercePools](docs/sdks/commercepools/README.md)

* [comCrmCommercePoolSelfServiceResourceActions](docs/sdks/commercepools/README.md#comcrmcommercepoolselfserviceresourceactions) - Commerce Pool Actions

### [Communications](docs/sdks/communications/README.md)

* [crmComCommunicationSelfServiceResourceGetSingle](docs/sdks/communications/README.md#crmcomcommunicationselfserviceresourcegetsingle) - Get Communications
* [crmComCommunicationSelfServiceResourceCommunicationActions](docs/sdks/communications/README.md#crmcomcommunicationselfserviceresourcecommunicationactions) - Communications Actions
* [crmComCommunicationSelfServiceResourceList](docs/sdks/communications/README.md#crmcomcommunicationselfserviceresourcelist) - List Communications
* [crmComPrintoutSelfServiceResourceOutput](docs/sdks/communications/README.md#crmcomprintoutselfserviceresourceoutput) - Printout

### [Communities](docs/sdks/communities/README.md)

* [comCrmContactSettingSelfServiceResourceListCommunityRelations](docs/sdks/communities/README.md#comcrmcontactsettingselfserviceresourcelistcommunityrelations) - List Community Relations
* [comCrmContactSelfServiceResourceGetContactCommunitySummaryResults](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactcommunitysummaryresults) - Get Conmmunity members
* [comCrmContactSelfServiceResourceGetCommunities](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcommunities) - List Contact's Communities
* [comCrmContactSelfServiceResourceLeaveCommunity](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceleavecommunity) - Leave from Community
* [comCrmContactSelfServiceResourceListContactGroups](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcelistcontactgroups) - List Contact's Groups
* [comCrmContactSelfServiceResourceUpdateContactGroupName](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceupdatecontactgroupname) - Update Contact Group Name
* [comCrmContactSelfServiceResourceListContactRelationship](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcelistcontactrelationship) - List Community People
* [comCrmContactSelfServiceResourceAddContactRelationship](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceaddcontactrelationship) - Add Community Person
* [comCrmContactSelfServiceResourceGetContactRelationship](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactrelationship) - Retrieve Community Person
* [comCrmContactSelfServiceResourceUpdateContactRelationship](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceupdatecontactrelationship) - Update Community Person
* [comCrmContactSelfServiceResourceRemoveContactRelationship](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceremovecontactrelationship) - Delete Community Person
* [comCrmContactSelfServiceResourceGetContactPersonAllowance](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactpersonallowance) - Retrieve Community Person product allowance
* [comCrmContactSelfServiceResourceAddContactRelationshipProductAllowance](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceaddcontactrelationshipproductallowance) - Add Community Person product allowance
* [comCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceupdatecontactrelationshipproductallowance) - Update Community Person product allowance
* [comCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceremovecontactrelationshipproductallowance) - Delete Community Person allowance product
* [comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactpersonremainingallowance) - Retrieve Community Person remaining product allowance

### [Contact](docs/sdks/contact/README.md)

* [comCrmContactSelfServiceResourceVerifyContactExists](docs/sdks/contact/README.md#comcrmcontactselfserviceresourceverifycontactexists) - Verify Contact Existence
* [comCrmContactSelfServiceResourceGetOIDCConfiguration](docs/sdks/contact/README.md#comcrmcontactselfserviceresourcegetoidcconfiguration) - OIDC Contact Authentication
* [registerContactSS](docs/sdks/contact/README.md#registercontactss) - Register Contact
* [getSingleContactSS](docs/sdks/contact/README.md#getsinglecontactss) - Get Contact
* [updateContactSS](docs/sdks/contact/README.md#updatecontactss) - Update Contact
* [comCrmContactSelfServiceResourceUnregisterContact](docs/sdks/contact/README.md#comcrmcontactselfserviceresourceunregistercontact) - Unregister Contact
* [comCrmAccountSelfServiceResourceExportStatement](docs/sdks/contact/README.md#comcrmaccountselfserviceresourceexportstatement) - Export Statement
* [comCrmContactSelfServiceResourceAction](docs/sdks/contact/README.md#comcrmcontactselfserviceresourceaction) - Perform Community Invitation Actions

### [ContactAccounts](docs/sdks/contactaccounts/README.md)

* [comCrmAccountSelfServiceResourceGetSingle](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcegetsingle) - Get Account
* [comCrmAccountSelfServiceResourceUpdateAccount](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourceupdateaccount) - Update Account
* [comCrmAccountSelfServiceResourceListAccountJournals](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcelistaccountjournals) - List Account Journals
* [comCrmAccountSelfServiceResourceList](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcelist) - List Contact Accounts
* [comCrmAccountSelfServiceResourceAddContactAccount](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourceaddcontactaccount) - Create account
* [comCrmAccountSelfServiceResourceGetAccountJournal](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcegetaccountjournal) - Get Account Journal

### [ContactAddresses](docs/sdks/contactaddresses/README.md)

* [listContactAddressesSS](docs/sdks/contactaddresses/README.md#listcontactaddressesss) - List Contact Addresses
* [addContactAddessSS](docs/sdks/contactaddresses/README.md#addcontactaddessss) - Add Contact Address
* [updateContactAddressSS](docs/sdks/contactaddresses/README.md#updatecontactaddressss) - Update Contact Address
* [deleteContactAddressSS](docs/sdks/contactaddresses/README.md#deletecontactaddressss) - Delete Contact Address

### [ContactAnalytics](docs/sdks/contactanalytics/README.md)

* [comCrmContactSelfServiceAnalyticsResourceGetAnalytics](docs/sdks/contactanalytics/README.md#comcrmcontactselfserviceanalyticsresourcegetanalytics) - Get Contact Analytics

### [ContactAttachments](docs/sdks/contactattachments/README.md)

* [comCrmContactSelfServiceResourceGetFiles](docs/sdks/contactattachments/README.md#comcrmcontactselfserviceresourcegetfiles) - List Contact Attachments
* [comCrmContactSelfServiceResourceCreateFile](docs/sdks/contactattachments/README.md#comcrmcontactselfserviceresourcecreatefile) - Add Contact Attachment
* [comCrmContactSelfServiceResourceRemoveFile](docs/sdks/contactattachments/README.md#comcrmcontactselfserviceresourceremovefile) - Delete Contact Attachment

### [ContactDevices](docs/sdks/contactdevices/README.md)

* [comCrmDeviceSelfServiceResourceGetContactDevices](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourcegetcontactdevices) - List Devices
* [comCrmDeviceSelfServiceResourceAddContactDevice](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourceaddcontactdevice) - Register Device
* [comCrmDeviceSelfServiceResourceListDeviceMeterReadings](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourcelistdevicemeterreadings) - List Device Meter Readings
* [comCrmDeviceSelfServiceResourceCreateDeviceMeterReading](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourcecreatedevicemeterreading) - Create Device Meter Reading
* [comCrmDeviceSelfServiceResourceRemoveContactDevice](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourceremovecontactdevice) - Delete Contact Devices
* [comCrmDeviceSelfServiceResourceUpdateDevice](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourceupdatedevice) - Update Device

### [ContactDonations](docs/sdks/contactdonations/README.md)

* [comCrmContactSelfServiceResourceListContactDonations](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourcelistcontactdonations) - List Contact Donation Offers
* [comCrmContactSelfServiceResourceOptInDonations](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourceoptindonations) - Contact Donation Actions
* [comCrmContactDonationSelfServiceResourceListContactDonationsHistory](docs/sdks/contactdonations/README.md#comcrmcontactdonationselfserviceresourcelistcontactdonationshistory) - List Contact Donation Offers History
* [comCrmContactSelfServiceResourceUpdateDonations](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourceupdatedonations) - Update donation offer preferences
* [comCrmContactSelfServiceResourceOptOutDonations](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourceoptoutdonations) - Opt out from Donation offer

### [ContactFinancials](docs/sdks/contactfinancials/README.md)

* [comCrmContactSelfServiceResourceGetClientToken](docs/sdks/contactfinancials/README.md#comcrmcontactselfserviceresourcegetclienttoken) - Get a Contact Client Token
* [comCrmPaymentIntentSelfServiceResourceSetUpIntents](docs/sdks/contactfinancials/README.md#comcrmpaymentintentselfserviceresourcesetupintents) - Create Intent
* [comCrmPaymentSelfServiceResourceCreate](docs/sdks/contactfinancials/README.md#comcrmpaymentselfserviceresourcecreate) - Create Payment
* [comCrmPayoutSelfServiceResourceCreate](docs/sdks/contactfinancials/README.md#comcrmpayoutselfserviceresourcecreate) - Create Payout
* [comCrmSettlementTransactionSelfServiceResourceList](docs/sdks/contactfinancials/README.md#comcrmsettlementtransactionselfserviceresourcelist) - Get Settlement Transactions
* [comCrmSettlementTransactionSelfServiceResourceGetMetrics](docs/sdks/contactfinancials/README.md#comcrmsettlementtransactionselfserviceresourcegetmetrics) - Get Settlement Transactions Metrics
* [comCrmTopUpSelfServiceResourceCreate](docs/sdks/contactfinancials/README.md#comcrmtopupselfserviceresourcecreate) - Create Top-up
* [comCrmTransferSelfServiceResourceCreate](docs/sdks/contactfinancials/README.md#comcrmtransferselfserviceresourcecreate) - Transfer Money
* [comCrmTransferSelfServiceResourceCreateTransferBulk](docs/sdks/contactfinancials/README.md#comcrmtransferselfserviceresourcecreatetransferbulk) - Transfer Money in Bulk

### [ContactImages](docs/sdks/contactimages/README.md)

* [comCrmContactSelfServiceResourceUploadImage](docs/sdks/contactimages/README.md#comcrmcontactselfserviceresourceuploadimage) - Upload Image
* [comCrmContactSelfServiceResourceDeleteImage](docs/sdks/contactimages/README.md#comcrmcontactselfserviceresourcedeleteimage) - Delete Contact Image

### [ContactMedia](docs/sdks/contactmedia/README.md)

* [comCrmContactSelfServiceMediaResourceSign](docs/sdks/contactmedia/README.md#comcrmcontactselfservicemediaresourcesign) - Create a Self Service V2 Media Upload Signature

### [ContactOrganisations](docs/sdks/contactorganisations/README.md)

* [comCrmContactSelfServiceResourceGetOrganisations](docs/sdks/contactorganisations/README.md#comcrmcontactselfserviceresourcegetorganisations) - Get Contact Organisations
* [signUpOutOrganisationSS](docs/sdks/contactorganisations/README.md#signupoutorganisationss) - Sign Up/Out Organisation

### [ContactPaymentMethods](docs/sdks/contactpaymentmethods/README.md)

* [comCrmContactSelfServiceResourceGetPaymentMethods](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourcegetpaymentmethods) - List Payment Methods
* [comCrmContactSelfServiceResourceAddPaymentMethod](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourceaddpaymentmethod) - Add Payment Method
* [comCrmContactSelfServiceResourceUpdatePaymentMethod](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourceupdatepaymentmethod) - Update Payment Method
* [comCrmContactSelfServiceResourceDeletePaymentMethod](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourcedeletepaymentmethod) - Remove Payment Method

### [ContactPreferences](docs/sdks/contactpreferences/README.md)

* [getContactPreferredOrganisationSS](docs/sdks/contactpreferences/README.md#getcontactpreferredorganisationss) - Get Contact Preferred Organisation
* [addContactPreferredOrganisationSS](docs/sdks/contactpreferences/README.md#addcontactpreferredorganisationss) - Add Contact Preferred Organisation

### [ContactRewards](docs/sdks/contactrewards/README.md)

* [comCrmContactSelfServiceResourceVerifySignUp](docs/sdks/contactrewards/README.md#comcrmcontactselfserviceresourceverifysignup) - Verify Closed Loop Scheme Request
* [comCrmContactSelfServiceResourceSignUpOutScheme](docs/sdks/contactrewards/README.md#comcrmcontactselfserviceresourcesignupoutscheme) - Contact Reward Schemes Actions
* [comCrmContactSelfServiceResourceGetSingleWithRewards](docs/sdks/contactrewards/README.md#comcrmcontactselfserviceresourcegetsinglewithrewards) - Get Contact Rewards

### [ContactTokens](docs/sdks/contacttokens/README.md)

* [listContactTokensSS](docs/sdks/contacttokens/README.md#listcontacttokensss) - List Contact Tokens
* [addContactTokenSS](docs/sdks/contacttokens/README.md#addcontacttokenss) - Request Contact Token

### [ContactWallet](docs/sdks/contactwallet/README.md)

* [comCrmContactSelfServiceResourceSetUpWallet](docs/sdks/contactwallet/README.md#comcrmcontactselfserviceresourcesetupwallet) - Create Wallet
* [comCrmWalletSelfServiceResourceRequestOTP](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcerequestotp) - Request Wallet One Time Password
* [comCrmWalletSelfServiceResourceVerifyWalletExists](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourceverifywalletexists) - Verify Wallet identity Existence
* [comCrmWalletSelfServiceResourceGetSingle](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetsingle) - Get Wallet
* [comCrmWalletSelfServiceResourceUpdate](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourceupdate) - Update Wallet
* [comCrmWalletSelfServiceResourceGetWalletCode](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwalletcode) - Get Wallet Code
* [comCrmWalletSelfServiceResourceGetBalances](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetbalances) - List Wallet Commerce Balances
* [comCrmWalletSelfServiceResourceListWalletJournals](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcelistwalletjournals) - List Wallet Journals
* [comCrmWalletSelfServiceResourceGetWalletLimits](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwalletlimits) - Get Wallet Limits
* [comCrmWalletSelfServiceResourceUpdateLimits](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourceupdatelimits) - Update Wallet Limits
* [comCrmWalletSelfServiceResourceGetWalletSummarisedTotals](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwalletsummarisedtotals) - List Wallet Summarised Totals
* [comCrmWalletSelfServiceResourceGetWalletTopUpSettings](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwallettopupsettings) - Get Wallet Top-up Settings
* [comCrmWalletSelfServiceResourceGetTransactions](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegettransactions) - List Wallet (Journal) Transactions

### [Contacts](docs/sdks/contacts/README.md)

* [comCrmContactSelfServiceResourceGetContactSharedDevices](docs/sdks/contacts/README.md#comcrmcontactselfserviceresourcegetcontactshareddevices) - List Contact Shared Devices

### [Donations](docs/sdks/donations/README.md)

* [comCrmRewardOfferDonationsSelfServiceResourceList](docs/sdks/donations/README.md#comcrmrewardofferdonationsselfserviceresourcelist) - Search Donation Offers
* [comCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs](docs/sdks/donations/README.md#comcrmrewardofferdonationsselfserviceresourcelistcharityorgs) - List Charity Organisations
* [comCrmRewardOfferDonationsSelfServiceResourceGetSingle](docs/sdks/donations/README.md#comcrmrewardofferdonationsselfserviceresourcegetsingle) - Get Donation Offer

### [Estimates](docs/sdks/estimates/README.md)

* [comCrmEstimateSelfServiceResourceEstimateInvoicing](docs/sdks/estimates/README.md#comcrmestimateselfserviceresourceestimateinvoicing) - Invoicing
* [comCrmEstimateOrderSelfServiceResourceEstimateOrder](docs/sdks/estimates/README.md#comcrmestimateorderselfserviceresourceestimateorder) - Order Preview

### [HostedPages](docs/sdks/hostedpages/README.md)

* [comCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegenerategiftpasspaymentform) - Get Gift Pass Payment Form
* [comCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegenerateaddpaymentmethodform) - Add Payment Method
* [comCrmHostedPagesSelfServiceResourceGeneratePaymentForm](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegeneratepaymentform) - Payment Form
* [comCrmHostedPagesSelfServiceResourceGeneratePayoutForm](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegeneratepayoutform) - Payout Form

### [MobilePassCards](docs/sdks/mobilepasscards/README.md)

* [comCrmWalletPassesSelfServiceResourceGetAndroidWalletPass](docs/sdks/mobilepasscards/README.md#comcrmwalletpassesselfserviceresourcegetandroidwalletpass) - Get Android Wallet Pass
* [comCrmWalletPassesSelfServiceResourceGetApplePass](docs/sdks/mobilepasscards/README.md#comcrmwalletpassesselfserviceresourcegetapplepass) - Get Apple Pass
* [comCrmWalletPassesSelfServiceResourceGetGooglePass](docs/sdks/mobilepasscards/README.md#comcrmwalletpassesselfserviceresourcegetgooglepass) - Get Google Pass

### [OrderCatalogues](docs/sdks/ordercatalogues/README.md)

* [comCrmOrderCatalogSelfServiceResourceList](docs/sdks/ordercatalogues/README.md#comcrmordercatalogselfserviceresourcelist) - List Order Catalogues
* [comCrmOrderCatalogSelfServiceResourceListCategories](docs/sdks/ordercatalogues/README.md#comcrmordercatalogselfserviceresourcelistcategories) - List Order Catalogue Categories

### [Orders](docs/sdks/orders/README.md)

* [comCrmOrderSelfServiceResourceListOrders](docs/sdks/orders/README.md#comcrmorderselfserviceresourcelistorders) - List Orders
* [comCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder](docs/sdks/orders/README.md#comcrmestimateorderfulfillmentselfserviceresourceestimateorder) - Order Fulfillment
* [comCrmOrderSelfServiceResourceCreateOrder](docs/sdks/orders/README.md#comcrmorderselfserviceresourcecreateorder) - Submit Order
* [comCrmOrderSelfServiceResourceGetOrder](docs/sdks/orders/README.md#comcrmorderselfserviceresourcegetorder) - Get Order
* [comCrmOrderSelfServiceResourcePerformOrderActions](docs/sdks/orders/README.md#comcrmorderselfserviceresourceperformorderactions) - Perform Order Actions

### [Organisations](docs/sdks/organisations/README.md)

* [comCrmBusinessActivitySelfServiceResourceListBusinessActivities](docs/sdks/organisations/README.md#comcrmbusinessactivityselfserviceresourcelistbusinessactivities) - List Business Activities
* [comCrmLocationSelfServiceResourceList](docs/sdks/organisations/README.md#comcrmlocationselfserviceresourcelist) - Locations
* [comCrmLocationSelfServiceResourceListTowns](docs/sdks/organisations/README.md#comcrmlocationselfserviceresourcelisttowns) - Locations
* [comCrmOrganisationSelfServiceResourceGetSingle](docs/sdks/organisations/README.md#comcrmorganisationselfserviceresourcegetsingle) - Get Organisation
* [comCrmOrganisationSelfServiceResourceList](docs/sdks/organisations/README.md#comcrmorganisationselfserviceresourcelist) - Search Organisations
* [comCrmOrganisationSelfServiceResourceSwitchOrganisation](docs/sdks/organisations/README.md#comcrmorganisationselfserviceresourceswitchorganisation) - Switch Organisations
* [comCrmMerchantSelfServiceResourceList](docs/sdks/organisations/README.md#comcrmmerchantselfserviceresourcelist) - Participating Merchants

### [Passes](docs/sdks/passes/README.md)

* [comCrmPassPlanSelfServiceResourceListPassTypes](docs/sdks/passes/README.md#comcrmpassplanselfserviceresourcelistpasstypes) - List Pass Plans
* [comCrmPassSelfServiceResourceRedeemPass](docs/sdks/passes/README.md#comcrmpassselfserviceresourceredeempass) - Redeem Pass
* [comCrmPassSelfServiceResourceViewPromoPass](docs/sdks/passes/README.md#comcrmpassselfserviceresourceviewpromopass) - View promo pass

### [~~PaymentForms~~](docs/sdks/paymentforms/README.md)

* [~~comCrmPaymentFormSelfServiceResourceGenerateAddCardForm~~](docs/sdks/paymentforms/README.md#comcrmpaymentformselfserviceresourcegenerateaddcardform) - Add Card :warning: **Deprecated**
* [~~comCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm~~](docs/sdks/paymentforms/README.md#comcrmpaymentformselfserviceresourcegeneratepasspaymentform) - Get Gift Pass Payment Form :warning: **Deprecated**
* [~~comCrmPaymentFormSelfServiceResourceGeneratePaymentForm~~](docs/sdks/paymentforms/README.md#comcrmpaymentformselfserviceresourcegeneratepaymentform) - Payment Form :warning: **Deprecated**

### [~~PayoutForms~~](docs/sdks/payoutforms/README.md)

* [~~comCrmPayoutFormSelfServiceResourceGeneratePayoutForm~~](docs/sdks/payoutforms/README.md#comcrmpayoutformselfserviceresourcegeneratepayoutform) - Payout Form :warning: **Deprecated**

### [Platform](docs/sdks/platform/README.md)

* [comCrmApplicationSelfServiceResourceGetApplication](docs/sdks/platform/README.md#comcrmapplicationselfserviceresourcegetapplication) - Get Application
* [comCrmApplicationSelfServiceResourceList](docs/sdks/platform/README.md#comcrmapplicationselfserviceresourcelist) - Integrations
* [comCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations](docs/sdks/platform/README.md#comcrmapplicationselfserviceresourcegetapplicationembeddedlinkstranslations) - Get Application Embedded Links Translations
* [comCrmCustomFieldSelfServiceResourceListCustomFields](docs/sdks/platform/README.md#comcrmcustomfieldselfserviceresourcelistcustomfields) - List Custom Fields
* [comCrmFileSelfServiceResourceGetFile](docs/sdks/platform/README.md#comcrmfileselfserviceresourcegetfile) - Get File
* [comCrmFileSelfServiceResourceDeleteFile](docs/sdks/platform/README.md#comcrmfileselfserviceresourcedeletefile) - Delete File
* [comCrmIndustrySelfServiceResourceListIndustries](docs/sdks/platform/README.md#comcrmindustryselfserviceresourcelistindustries) - List Industries
* [comCrmLandingPageSelfServiceResourceGetSingleLandingPage](docs/sdks/platform/README.md#comcrmlandingpageselfserviceresourcegetsinglelandingpage) - Get Landing Pages
* [comCrmLanguageSelfServiceResourceGetSupportedLanguages](docs/sdks/platform/README.md#comcrmlanguageselfserviceresourcegetsupportedlanguages) - List Languages
* [comCrmSubIndustrySelfServiceResourceListSubIndustrySectors](docs/sdks/platform/README.md#comcrmsubindustryselfserviceresourcelistsubindustrysectors) - List Sub-Industries
* [comCrmFileSelfServiceResourceUploadFile](docs/sdks/platform/README.md#comcrmfileselfserviceresourceuploadfile) - Upload File

### [ProductCatalogue](docs/sdks/productcatalogue/README.md)

* [comCrmProductSelfServiceResourceListProducts](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcelistproducts) - Search Products
* [comCrmProductSelfServiceResourceGetProduct](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcegetproduct) - Get Product
* [comCrmProductSelfServiceResourceGetProductComponents](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcegetproductcomponents) - Get Product Components
* [comCrmProductSelfServiceResourceGetProductVariations](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcegetproductvariations) - Get Product Variants

### [Promotions](docs/sdks/promotions/README.md)

* [comCrmPromotionSelfServiceResourceList](docs/sdks/promotions/README.md#comcrmpromotionselfserviceresourcelist) - List Promotions
* [comCrmPromotionSelfServiceResourceGetSingle](docs/sdks/promotions/README.md#comcrmpromotionselfserviceresourcegetsingle) - Get Promotion

### [ProvisioningProviders](docs/sdks/provisioningproviders/README.md)

* [comCrmServiceCommandsSelfServiceResourceGetServiceCommands](docs/sdks/provisioningproviders/README.md#comcrmservicecommandsselfserviceresourcegetservicecommands) - Get Service Commands
* [comCrmServiceCommandsSelfServiceResourceSendServiceCommands](docs/sdks/provisioningproviders/README.md#comcrmservicecommandsselfserviceresourcesendservicecommands) - Send Service Command

### [PurchaseCustomerEvents](docs/sdks/purchasecustomerevents/README.md)

* [comCrmPurchaseCustomerEventSelfServiceResourceListPurchases](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcelistpurchases) - Search Contact Purchases
* [comCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcereclaimpurchase) - Reclaim Purchase To Contact
* [comCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcegetsinglepurchase) - Get Purchase
* [comCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcegetpurchaserewardtransactions) - List Purchase Rewards Breakdown

### [Recommendations](docs/sdks/recommendations/README.md)

* [comCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation](docs/sdks/recommendations/README.md#comcrmorderproductrecommendationselfserviceresourcegetorderproductrecommendation) - Order Product Recommendation Self-Service
* [comCrmProductRecommendationSelfServiceResourceGetProductRecommendation](docs/sdks/recommendations/README.md#comcrmproductrecommendationselfserviceresourcegetproductrecommendation) - Product Recommendation
* [comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation](docs/sdks/recommendations/README.md#comcrmservicerecommendationselfserviceresourcegetservicerecommendation) - Service Recommendation

### [ReferralCustomerEvents](docs/sdks/referralcustomerevents/README.md)

* [comCrmReferralCustomerEventSelfServiceResourceCreateReferral](docs/sdks/referralcustomerevents/README.md#comcrmreferralcustomereventselfserviceresourcecreatereferral) - Create Referral
* [comCrmReferralCustomerEventSelfServiceResourceReferralActions](docs/sdks/referralcustomerevents/README.md#comcrmreferralcustomereventselfserviceresourcereferralactions) - Referral Actions

### [RewardOffers](docs/sdks/rewardoffers/README.md)

* [comCrmRewardOfferSelfServiceResourceList](docs/sdks/rewardoffers/README.md#comcrmrewardofferselfserviceresourcelist) - Search Reward Offers
* [comCrmRewardOfferSelfServiceResourceGetSingle](docs/sdks/rewardoffers/README.md#comcrmrewardofferselfserviceresourcegetsingle) - Get Reward Offer
* [comCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance](docs/sdks/rewardoffers/README.md#comcrmrewardofferselfserviceresourcegetrewardofferperformance) - Get Reward Offer Performance

### [RewardSchemes](docs/sdks/rewardschemes/README.md)

* [comCrmRewardSchemeSelfServiceResourceList](docs/sdks/rewardschemes/README.md#comcrmrewardschemeselfserviceresourcelist) - Search Reward Schemes

### [ServiceRequests](docs/sdks/servicerequests/README.md)

* [comCrmServiceRequestSelfServiceResourceList](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcelist) - List Service Requests
* [comCrmServiceRequestSelfServiceResourceCreate](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcecreate) - Create Service Request
* [comCrmQueueSelfServiceResourceList](docs/sdks/servicerequests/README.md#comcrmqueueselfserviceresourcelist) - List Service Request Queues
* [comCrmServiceRequestSelfServiceResourceGetFiles](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcegetfiles) - List Service Request Attachments
* [comCrmServiceRequestSelfServiceResourceCreateServiceRequestFile](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcecreateservicerequestfile) - Add Service Request Attachment
* [comCrmServiceRequestSelfServiceResourceRemoveFile](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourceremovefile) - Delete Service Request Attachment
* [comCrmServiceRequestSelfServiceResourceGetNotes](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcegetnotes) - List Service Request Note
* [comCrmServiceRequestSelfServiceResourceCreateNote](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcecreatenote) - Create Service Request Note

### [Settings](docs/sdks/settings/README.md)

* [comCrmNameDayRulesSelfServiceResourceListNameDayRules](docs/sdks/settings/README.md#comcrmnamedayrulesselfserviceresourcelistnamedayrules) - List Name Day Rules
* [comCrmProductBrandSelfServiceResourceGetProductBrands](docs/sdks/settings/README.md#comcrmproductbrandselfserviceresourcegetproductbrands) - List Product Brands
* [comCrmProductCategorySelfServiceResourceListProductCategories](docs/sdks/settings/README.md#comcrmproductcategoryselfserviceresourcelistproductcategories) - List Product Categories
* [comCrmProductTypeSelfServiceResourceListProductTypes](docs/sdks/settings/README.md#comcrmproducttypeselfserviceresourcelistproducttypes) - List Product Types

### [Subscriptions](docs/sdks/subscriptions/README.md)

* [comCrmSubscriptionSelfServiceResourceListSubscriptionServices](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistsubscriptionservices) - List Contact Services
* [comCrmSubscriptionSelfServiceResourceAddService](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourceaddservice) - Add Service
* [comCrmSubscriptionSelfServiceResourceListContactSubscriptions](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistcontactsubscriptions) - List Contact Subscriptions
* [comCrmSubscriptionSelfServiceResourceListContactSubscriptionActions](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistcontactsubscriptionactions) - List Contact Subscription Actions
* [comCrmEstimateSubscriptionSelfServiceResourceEstimateBilling](docs/sdks/subscriptions/README.md#comcrmestimatesubscriptionselfserviceresourceestimatebilling) - Billing
* [comCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription](docs/sdks/subscriptions/README.md#comcrmestimatesubscriptionselfserviceresourceestimatesubscription) - Service Delivery
* [comCrmSubscriptionSelfServiceResourceChangeService](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcechangeservice) - Update Service
* [comCrmSubscriptionSelfServiceResourceListServiceDevices](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistservicedevices) - Get Service Devices
* [comCrmSubscriptionSelfServiceResourceListSubscriptionActions](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistsubscriptionactions) - List Subscription Actions
* [comCrmSubscriptionSelfServiceResourceGetSubscriptionAction](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcegetsubscriptionaction) - Get Subscription Action
* [comCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourceupdatesubscriptionaction) - Update Subscription Action
* [comCrmSubscriptionSelfServiceResourceChange](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcechange) - Update Subscription

### [Tags](docs/sdks/tags/README.md)

* [comCrmOrganisationTagSelfServiceResourceListOrganisationTags](docs/sdks/tags/README.md#comcrmorganisationtagselfserviceresourcelistorganisationtags) - List Organisation Tags
* [comCrmTagSelfServiceResourceListTags](docs/sdks/tags/README.md#comcrmtagselfserviceresourcelisttags) - List Tags

### [Usage](docs/sdks/usage/README.md)

* [comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords](docs/sdks/usage/README.md#comcrmusagedetailrecordselfserviceresourcelistusagedetailrecords) - List Usage Records
* [comCrmUsageDetailRecordSelfServiceResourceGetMetrics](docs/sdks/usage/README.md#comcrmusagedetailrecordselfserviceresourcegetmetrics) - Get Usage Records Metrics
* [comCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance](docs/sdks/usage/README.md#comcrmestimateallowanceselfserviceresourceestimatesallowance) - Authorise Usage Consumption

### [Wifi](docs/sdks/wifi/README.md)

* [comCrmSelfServiceWifiAuthorizationResourceAuthorizeContact](docs/sdks/wifi/README.md#comcrmselfservicewifiauthorizationresourceauthorizecontact) - Contact WiFi Authorization

</details>
<!-- End Available Resources and Operations [operations] -->

<!-- Start Standalone functions [standalone-funcs] -->
## Standalone functions

All the methods listed above are available as standalone functions. These
functions are ideal for use in applications running in the browser, serverless
runtimes or other environments where application bundle size is a primary
concern. When using a bundler to build your application, all unused
functionality will be either excluded from the final bundle or tree-shaken away.

To read more about standalone functions, check [FUNCTIONS.md](./FUNCTIONS.md).

<details>

<summary>Available standalone functions</summary>

- [`addressLookupComCrmAddressRegistrySelfServiceResourceGetAddress`](docs/sdks/addresslookup/README.md#comcrmaddressregistryselfserviceresourcegetaddress) - Get Address
- [`addressLookupComCrmAddressRegistrySelfServiceResourceList`](docs/sdks/addresslookup/README.md#comcrmaddressregistryselfserviceresourcelist) - Search Addresses
- [`approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequest`](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourceacceptapprovalrequest) - Approve an Approval Request
- [`approvalRequestsComCrmApprovalRequestSelfServiceResourceAcceptApprovalRequestAction`](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourceacceptapprovalrequestaction) - Approve an Approval Request
- [`approvalRequestsComCrmApprovalRequestSelfServiceResourceList`](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourcelist) - List Approval Requests
- [`approvalRequestsComCrmApprovalRequestSelfServiceResourcePerformActions`](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourceperformactions) - Perform Approval Request Actions
- [`approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequest`](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourcerejectapprovalrequest) - Show the Reject an Approval Request Form
- [`approvalRequestsComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestAction`](docs/sdks/approvalrequests/README.md#comcrmapprovalrequestselfserviceresourcerejectapprovalrequestaction) - Reject an Approval Request
- [`authenticationAddContactIdentitySS`](docs/sdks/authentication/README.md#addcontactidentityss) - Add Contact Identity
- [`authenticationComCrmContactSelfServiceResourceAuthenticate`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceauthenticate) - Contact Authentication
- [`authenticationComCrmContactSelfServiceResourceChangeForgottenPassword`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcechangeforgottenpassword) - Change Forgotten Password
- [`authenticationComCrmContactSelfServiceResourceChangePassword`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcechangepassword) - Change Password
- [`authenticationComCrmContactSelfServiceResourceEmailVerification`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceemailverification) - Request Email Verification
- [`authenticationComCrmContactSelfServiceResourceForgotPassword`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceforgotpassword) - Forgot Password
- [`authenticationComCrmContactSelfServiceResourceRefresh`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcerefresh) - Refresh Contact Token
- [`authenticationComCrmContactSelfServiceResourceRequestOTP`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcerequestotp) - Request One Time Password
- [`authenticationComCrmContactSelfServiceResourceSignOut`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcesignout) - Sign Out Contact
- [`authenticationComCrmContactSelfServiceResourceSwitchContact`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceswitchcontact) - Contact Switch
- [`authenticationComCrmContactSelfServiceResourceValidateOTP`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourcevalidateotp) - Validate One Time Password
- [`authenticationComCrmContactSelfServiceResourceVerifyContactEmail`](docs/sdks/authentication/README.md#comcrmcontactselfserviceresourceverifycontactemail) - Verify Contact Email
- [`commercePoolsComCrmCommercePoolSelfServiceResourceActions`](docs/sdks/commercepools/README.md#comcrmcommercepoolselfserviceresourceactions) - Commerce Pool Actions
- [`communicationsCrmComCommunicationSelfServiceResourceCommunicationActions`](docs/sdks/communications/README.md#crmcomcommunicationselfserviceresourcecommunicationactions) - Communications Actions
- [`communicationsCrmComCommunicationSelfServiceResourceGetSingle`](docs/sdks/communications/README.md#crmcomcommunicationselfserviceresourcegetsingle) - Get Communications
- [`communicationsCrmComCommunicationSelfServiceResourceList`](docs/sdks/communications/README.md#crmcomcommunicationselfserviceresourcelist) - List Communications
- [`communicationsCrmComPrintoutSelfServiceResourceOutput`](docs/sdks/communications/README.md#crmcomprintoutselfserviceresourceoutput) - Printout
- [`communitiesComCrmContactSelfServiceResourceAddContactRelationship`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceaddcontactrelationship) - Add Community Person
- [`communitiesComCrmContactSelfServiceResourceAddContactRelationshipProductAllowance`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceaddcontactrelationshipproductallowance) - Add Community Person product allowance
- [`communitiesComCrmContactSelfServiceResourceGetCommunities`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcommunities) - List Contact's Communities
- [`communitiesComCrmContactSelfServiceResourceGetContactCommunitySummaryResults`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactcommunitysummaryresults) - Get Conmmunity members
- [`communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactpersonallowance) - Retrieve Community Person product allowance
- [`communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactpersonremainingallowance) - Retrieve Community Person remaining product allowance
- [`communitiesComCrmContactSelfServiceResourceGetContactRelationship`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcegetcontactrelationship) - Retrieve Community Person
- [`communitiesComCrmContactSelfServiceResourceLeaveCommunity`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceleavecommunity) - Leave from Community
- [`communitiesComCrmContactSelfServiceResourceListContactGroups`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcelistcontactgroups) - List Contact's Groups
- [`communitiesComCrmContactSelfServiceResourceListContactRelationship`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourcelistcontactrelationship) - List Community People
- [`communitiesComCrmContactSelfServiceResourceRemoveContactRelationship`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceremovecontactrelationship) - Delete Community Person
- [`communitiesComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceremovecontactrelationshipproductallowance) - Delete Community Person allowance product
- [`communitiesComCrmContactSelfServiceResourceUpdateContactGroupName`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceupdatecontactgroupname) - Update Contact Group Name
- [`communitiesComCrmContactSelfServiceResourceUpdateContactRelationship`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceupdatecontactrelationship) - Update Community Person
- [`communitiesComCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance`](docs/sdks/communities/README.md#comcrmcontactselfserviceresourceupdatecontactrelationshipproductallowance) - Update Community Person product allowance
- [`communitiesComCrmContactSettingSelfServiceResourceListCommunityRelations`](docs/sdks/communities/README.md#comcrmcontactsettingselfserviceresourcelistcommunityrelations) - List Community Relations
- [`contactAccountsComCrmAccountSelfServiceResourceAddContactAccount`](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourceaddcontactaccount) - Create account
- [`contactAccountsComCrmAccountSelfServiceResourceGetAccountJournal`](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcegetaccountjournal) - Get Account Journal
- [`contactAccountsComCrmAccountSelfServiceResourceGetSingle`](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcegetsingle) - Get Account
- [`contactAccountsComCrmAccountSelfServiceResourceList`](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcelist) - List Contact Accounts
- [`contactAccountsComCrmAccountSelfServiceResourceListAccountJournals`](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourcelistaccountjournals) - List Account Journals
- [`contactAccountsComCrmAccountSelfServiceResourceUpdateAccount`](docs/sdks/contactaccounts/README.md#comcrmaccountselfserviceresourceupdateaccount) - Update Account
- [`contactAddressesAddContactAddessSS`](docs/sdks/contactaddresses/README.md#addcontactaddessss) - Add Contact Address
- [`contactAddressesDeleteContactAddressSS`](docs/sdks/contactaddresses/README.md#deletecontactaddressss) - Delete Contact Address
- [`contactAddressesListContactAddressesSS`](docs/sdks/contactaddresses/README.md#listcontactaddressesss) - List Contact Addresses
- [`contactAddressesUpdateContactAddressSS`](docs/sdks/contactaddresses/README.md#updatecontactaddressss) - Update Contact Address
- [`contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics`](docs/sdks/contactanalytics/README.md#comcrmcontactselfserviceanalyticsresourcegetanalytics) - Get Contact Analytics
- [`contactAttachmentsComCrmContactSelfServiceResourceCreateFile`](docs/sdks/contactattachments/README.md#comcrmcontactselfserviceresourcecreatefile) - Add Contact Attachment
- [`contactAttachmentsComCrmContactSelfServiceResourceGetFiles`](docs/sdks/contactattachments/README.md#comcrmcontactselfserviceresourcegetfiles) - List Contact Attachments
- [`contactAttachmentsComCrmContactSelfServiceResourceRemoveFile`](docs/sdks/contactattachments/README.md#comcrmcontactselfserviceresourceremovefile) - Delete Contact Attachment
- [`contactComCrmAccountSelfServiceResourceExportStatement`](docs/sdks/contact/README.md#comcrmaccountselfserviceresourceexportstatement) - Export Statement
- [`contactComCrmContactSelfServiceResourceAction`](docs/sdks/contact/README.md#comcrmcontactselfserviceresourceaction) - Perform Community Invitation Actions
- [`contactComCrmContactSelfServiceResourceGetOIDCConfiguration`](docs/sdks/contact/README.md#comcrmcontactselfserviceresourcegetoidcconfiguration) - OIDC Contact Authentication
- [`contactComCrmContactSelfServiceResourceUnregisterContact`](docs/sdks/contact/README.md#comcrmcontactselfserviceresourceunregistercontact) - Unregister Contact
- [`contactComCrmContactSelfServiceResourceVerifyContactExists`](docs/sdks/contact/README.md#comcrmcontactselfserviceresourceverifycontactexists) - Verify Contact Existence
- [`contactDevicesComCrmDeviceSelfServiceResourceAddContactDevice`](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourceaddcontactdevice) - Register Device
- [`contactDevicesComCrmDeviceSelfServiceResourceCreateDeviceMeterReading`](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourcecreatedevicemeterreading) - Create Device Meter Reading
- [`contactDevicesComCrmDeviceSelfServiceResourceGetContactDevices`](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourcegetcontactdevices) - List Devices
- [`contactDevicesComCrmDeviceSelfServiceResourceListDeviceMeterReadings`](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourcelistdevicemeterreadings) - List Device Meter Readings
- [`contactDevicesComCrmDeviceSelfServiceResourceRemoveContactDevice`](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourceremovecontactdevice) - Delete Contact Devices
- [`contactDevicesComCrmDeviceSelfServiceResourceUpdateDevice`](docs/sdks/contactdevices/README.md#comcrmdeviceselfserviceresourceupdatedevice) - Update Device
- [`contactDonationsComCrmContactDonationSelfServiceResourceListContactDonationsHistory`](docs/sdks/contactdonations/README.md#comcrmcontactdonationselfserviceresourcelistcontactdonationshistory) - List Contact Donation Offers History
- [`contactDonationsComCrmContactSelfServiceResourceListContactDonations`](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourcelistcontactdonations) - List Contact Donation Offers
- [`contactDonationsComCrmContactSelfServiceResourceOptInDonations`](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourceoptindonations) - Contact Donation Actions
- [`contactDonationsComCrmContactSelfServiceResourceOptOutDonations`](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourceoptoutdonations) - Opt out from Donation offer
- [`contactDonationsComCrmContactSelfServiceResourceUpdateDonations`](docs/sdks/contactdonations/README.md#comcrmcontactselfserviceresourceupdatedonations) - Update donation offer preferences
- [`contactFinancialsComCrmContactSelfServiceResourceGetClientToken`](docs/sdks/contactfinancials/README.md#comcrmcontactselfserviceresourcegetclienttoken) - Get a Contact Client Token
- [`contactFinancialsComCrmPaymentIntentSelfServiceResourceSetUpIntents`](docs/sdks/contactfinancials/README.md#comcrmpaymentintentselfserviceresourcesetupintents) - Create Intent
- [`contactFinancialsComCrmPaymentSelfServiceResourceCreate`](docs/sdks/contactfinancials/README.md#comcrmpaymentselfserviceresourcecreate) - Create Payment
- [`contactFinancialsComCrmPayoutSelfServiceResourceCreate`](docs/sdks/contactfinancials/README.md#comcrmpayoutselfserviceresourcecreate) - Create Payout
- [`contactFinancialsComCrmSettlementTransactionSelfServiceResourceGetMetrics`](docs/sdks/contactfinancials/README.md#comcrmsettlementtransactionselfserviceresourcegetmetrics) - Get Settlement Transactions Metrics
- [`contactFinancialsComCrmSettlementTransactionSelfServiceResourceList`](docs/sdks/contactfinancials/README.md#comcrmsettlementtransactionselfserviceresourcelist) - Get Settlement Transactions
- [`contactFinancialsComCrmTopUpSelfServiceResourceCreate`](docs/sdks/contactfinancials/README.md#comcrmtopupselfserviceresourcecreate) - Create Top-up
- [`contactFinancialsComCrmTransferSelfServiceResourceCreate`](docs/sdks/contactfinancials/README.md#comcrmtransferselfserviceresourcecreate) - Transfer Money
- [`contactFinancialsComCrmTransferSelfServiceResourceCreateTransferBulk`](docs/sdks/contactfinancials/README.md#comcrmtransferselfserviceresourcecreatetransferbulk) - Transfer Money in Bulk
- [`contactGetSingleContactSS`](docs/sdks/contact/README.md#getsinglecontactss) - Get Contact
- [`contactImagesComCrmContactSelfServiceResourceDeleteImage`](docs/sdks/contactimages/README.md#comcrmcontactselfserviceresourcedeleteimage) - Delete Contact Image
- [`contactImagesComCrmContactSelfServiceResourceUploadImage`](docs/sdks/contactimages/README.md#comcrmcontactselfserviceresourceuploadimage) - Upload Image
- [`contactMediaComCrmContactSelfServiceMediaResourceSign`](docs/sdks/contactmedia/README.md#comcrmcontactselfservicemediaresourcesign) - Create a Self Service V2 Media Upload Signature
- [`contactOrganisationsComCrmContactSelfServiceResourceGetOrganisations`](docs/sdks/contactorganisations/README.md#comcrmcontactselfserviceresourcegetorganisations) - Get Contact Organisations
- [`contactOrganisationsSignUpOutOrganisationSS`](docs/sdks/contactorganisations/README.md#signupoutorganisationss) - Sign Up/Out Organisation
- [`contactPaymentMethodsComCrmContactSelfServiceResourceAddPaymentMethod`](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourceaddpaymentmethod) - Add Payment Method
- [`contactPaymentMethodsComCrmContactSelfServiceResourceDeletePaymentMethod`](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourcedeletepaymentmethod) - Remove Payment Method
- [`contactPaymentMethodsComCrmContactSelfServiceResourceGetPaymentMethods`](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourcegetpaymentmethods) - List Payment Methods
- [`contactPaymentMethodsComCrmContactSelfServiceResourceUpdatePaymentMethod`](docs/sdks/contactpaymentmethods/README.md#comcrmcontactselfserviceresourceupdatepaymentmethod) - Update Payment Method
- [`contactPreferencesAddContactPreferredOrganisationSS`](docs/sdks/contactpreferences/README.md#addcontactpreferredorganisationss) - Add Contact Preferred Organisation
- [`contactPreferencesGetContactPreferredOrganisationSS`](docs/sdks/contactpreferences/README.md#getcontactpreferredorganisationss) - Get Contact Preferred Organisation
- [`contactRegisterContactSS`](docs/sdks/contact/README.md#registercontactss) - Register Contact
- [`contactRewardsComCrmContactSelfServiceResourceGetSingleWithRewards`](docs/sdks/contactrewards/README.md#comcrmcontactselfserviceresourcegetsinglewithrewards) - Get Contact Rewards
- [`contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme`](docs/sdks/contactrewards/README.md#comcrmcontactselfserviceresourcesignupoutscheme) - Contact Reward Schemes Actions
- [`contactRewardsComCrmContactSelfServiceResourceVerifySignUp`](docs/sdks/contactrewards/README.md#comcrmcontactselfserviceresourceverifysignup) - Verify Closed Loop Scheme Request
- [`contactsComCrmContactSelfServiceResourceGetContactSharedDevices`](docs/sdks/contacts/README.md#comcrmcontactselfserviceresourcegetcontactshareddevices) - List Contact Shared Devices
- [`contactTokensAddContactTokenSS`](docs/sdks/contacttokens/README.md#addcontacttokenss) - Request Contact Token
- [`contactTokensListContactTokensSS`](docs/sdks/contacttokens/README.md#listcontacttokensss) - List Contact Tokens
- [`contactUpdateContactSS`](docs/sdks/contact/README.md#updatecontactss) - Update Contact
- [`contactWalletComCrmContactSelfServiceResourceSetUpWallet`](docs/sdks/contactwallet/README.md#comcrmcontactselfserviceresourcesetupwallet) - Create Wallet
- [`contactWalletComCrmWalletSelfServiceResourceGetBalances`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetbalances) - List Wallet Commerce Balances
- [`contactWalletComCrmWalletSelfServiceResourceGetSingle`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetsingle) - Get Wallet
- [`contactWalletComCrmWalletSelfServiceResourceGetTransactions`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegettransactions) - List Wallet (Journal) Transactions
- [`contactWalletComCrmWalletSelfServiceResourceGetWalletCode`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwalletcode) - Get Wallet Code
- [`contactWalletComCrmWalletSelfServiceResourceGetWalletLimits`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwalletlimits) - Get Wallet Limits
- [`contactWalletComCrmWalletSelfServiceResourceGetWalletSummarisedTotals`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwalletsummarisedtotals) - List Wallet Summarised Totals
- [`contactWalletComCrmWalletSelfServiceResourceGetWalletTopUpSettings`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcegetwallettopupsettings) - Get Wallet Top-up Settings
- [`contactWalletComCrmWalletSelfServiceResourceListWalletJournals`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcelistwalletjournals) - List Wallet Journals
- [`contactWalletComCrmWalletSelfServiceResourceRequestOTP`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourcerequestotp) - Request Wallet One Time Password
- [`contactWalletComCrmWalletSelfServiceResourceUpdate`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourceupdate) - Update Wallet
- [`contactWalletComCrmWalletSelfServiceResourceUpdateLimits`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourceupdatelimits) - Update Wallet Limits
- [`contactWalletComCrmWalletSelfServiceResourceVerifyWalletExists`](docs/sdks/contactwallet/README.md#comcrmwalletselfserviceresourceverifywalletexists) - Verify Wallet identity Existence
- [`donationsComCrmRewardOfferDonationsSelfServiceResourceGetSingle`](docs/sdks/donations/README.md#comcrmrewardofferdonationsselfserviceresourcegetsingle) - Get Donation Offer
- [`donationsComCrmRewardOfferDonationsSelfServiceResourceList`](docs/sdks/donations/README.md#comcrmrewardofferdonationsselfserviceresourcelist) - Search Donation Offers
- [`donationsComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgs`](docs/sdks/donations/README.md#comcrmrewardofferdonationsselfserviceresourcelistcharityorgs) - List Charity Organisations
- [`estimatesComCrmEstimateOrderSelfServiceResourceEstimateOrder`](docs/sdks/estimates/README.md#comcrmestimateorderselfserviceresourceestimateorder) - Order Preview
- [`estimatesComCrmEstimateSelfServiceResourceEstimateInvoicing`](docs/sdks/estimates/README.md#comcrmestimateselfserviceresourceestimateinvoicing) - Invoicing
- [`hostedPagesComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm`](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegenerateaddpaymentmethodform) - Add Payment Method
- [`hostedPagesComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm`](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegenerategiftpasspaymentform) - Get Gift Pass Payment Form
- [`hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePaymentForm`](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegeneratepaymentform) - Payment Form
- [`hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePayoutForm`](docs/sdks/hostedpages/README.md#comcrmhostedpagesselfserviceresourcegeneratepayoutform) - Payout Form
- [`mobilePassCardsComCrmWalletPassesSelfServiceResourceGetAndroidWalletPass`](docs/sdks/mobilepasscards/README.md#comcrmwalletpassesselfserviceresourcegetandroidwalletpass) - Get Android Wallet Pass
- [`mobilePassCardsComCrmWalletPassesSelfServiceResourceGetApplePass`](docs/sdks/mobilepasscards/README.md#comcrmwalletpassesselfserviceresourcegetapplepass) - Get Apple Pass
- [`mobilePassCardsComCrmWalletPassesSelfServiceResourceGetGooglePass`](docs/sdks/mobilepasscards/README.md#comcrmwalletpassesselfserviceresourcegetgooglepass) - Get Google Pass
- [`orderCataloguesComCrmOrderCatalogSelfServiceResourceList`](docs/sdks/ordercatalogues/README.md#comcrmordercatalogselfserviceresourcelist) - List Order Catalogues
- [`orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories`](docs/sdks/ordercatalogues/README.md#comcrmordercatalogselfserviceresourcelistcategories) - List Order Catalogue Categories
- [`ordersComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder`](docs/sdks/orders/README.md#comcrmestimateorderfulfillmentselfserviceresourceestimateorder) - Order Fulfillment
- [`ordersComCrmOrderSelfServiceResourceCreateOrder`](docs/sdks/orders/README.md#comcrmorderselfserviceresourcecreateorder) - Submit Order
- [`ordersComCrmOrderSelfServiceResourceGetOrder`](docs/sdks/orders/README.md#comcrmorderselfserviceresourcegetorder) - Get Order
- [`ordersComCrmOrderSelfServiceResourceListOrders`](docs/sdks/orders/README.md#comcrmorderselfserviceresourcelistorders) - List Orders
- [`ordersComCrmOrderSelfServiceResourcePerformOrderActions`](docs/sdks/orders/README.md#comcrmorderselfserviceresourceperformorderactions) - Perform Order Actions
- [`organisationsComCrmBusinessActivitySelfServiceResourceListBusinessActivities`](docs/sdks/organisations/README.md#comcrmbusinessactivityselfserviceresourcelistbusinessactivities) - List Business Activities
- [`organisationsComCrmLocationSelfServiceResourceList`](docs/sdks/organisations/README.md#comcrmlocationselfserviceresourcelist) - Locations
- [`organisationsComCrmLocationSelfServiceResourceListTowns`](docs/sdks/organisations/README.md#comcrmlocationselfserviceresourcelisttowns) - Locations
- [`organisationsComCrmMerchantSelfServiceResourceList`](docs/sdks/organisations/README.md#comcrmmerchantselfserviceresourcelist) - Participating Merchants
- [`organisationsComCrmOrganisationSelfServiceResourceGetSingle`](docs/sdks/organisations/README.md#comcrmorganisationselfserviceresourcegetsingle) - Get Organisation
- [`organisationsComCrmOrganisationSelfServiceResourceList`](docs/sdks/organisations/README.md#comcrmorganisationselfserviceresourcelist) - Search Organisations
- [`organisationsComCrmOrganisationSelfServiceResourceSwitchOrganisation`](docs/sdks/organisations/README.md#comcrmorganisationselfserviceresourceswitchorganisation) - Switch Organisations
- [`passesComCrmPassPlanSelfServiceResourceListPassTypes`](docs/sdks/passes/README.md#comcrmpassplanselfserviceresourcelistpasstypes) - List Pass Plans
- [`passesComCrmPassSelfServiceResourceRedeemPass`](docs/sdks/passes/README.md#comcrmpassselfserviceresourceredeempass) - Redeem Pass
- [`passesComCrmPassSelfServiceResourceViewPromoPass`](docs/sdks/passes/README.md#comcrmpassselfserviceresourceviewpromopass) - View promo pass
- [`platformComCrmApplicationSelfServiceResourceGetApplication`](docs/sdks/platform/README.md#comcrmapplicationselfserviceresourcegetapplication) - Get Application
- [`platformComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslations`](docs/sdks/platform/README.md#comcrmapplicationselfserviceresourcegetapplicationembeddedlinkstranslations) - Get Application Embedded Links Translations
- [`platformComCrmApplicationSelfServiceResourceList`](docs/sdks/platform/README.md#comcrmapplicationselfserviceresourcelist) - Integrations
- [`platformComCrmCustomFieldSelfServiceResourceListCustomFields`](docs/sdks/platform/README.md#comcrmcustomfieldselfserviceresourcelistcustomfields) - List Custom Fields
- [`platformComCrmFileSelfServiceResourceDeleteFile`](docs/sdks/platform/README.md#comcrmfileselfserviceresourcedeletefile) - Delete File
- [`platformComCrmFileSelfServiceResourceGetFile`](docs/sdks/platform/README.md#comcrmfileselfserviceresourcegetfile) - Get File
- [`platformComCrmFileSelfServiceResourceUploadFile`](docs/sdks/platform/README.md#comcrmfileselfserviceresourceuploadfile) - Upload File
- [`platformComCrmIndustrySelfServiceResourceListIndustries`](docs/sdks/platform/README.md#comcrmindustryselfserviceresourcelistindustries) - List Industries
- [`platformComCrmLandingPageSelfServiceResourceGetSingleLandingPage`](docs/sdks/platform/README.md#comcrmlandingpageselfserviceresourcegetsinglelandingpage) - Get Landing Pages
- [`platformComCrmLanguageSelfServiceResourceGetSupportedLanguages`](docs/sdks/platform/README.md#comcrmlanguageselfserviceresourcegetsupportedlanguages) - List Languages
- [`platformComCrmSubIndustrySelfServiceResourceListSubIndustrySectors`](docs/sdks/platform/README.md#comcrmsubindustryselfserviceresourcelistsubindustrysectors) - List Sub-Industries
- [`productCatalogueComCrmProductSelfServiceResourceGetProduct`](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcegetproduct) - Get Product
- [`productCatalogueComCrmProductSelfServiceResourceGetProductComponents`](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcegetproductcomponents) - Get Product Components
- [`productCatalogueComCrmProductSelfServiceResourceGetProductVariations`](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcegetproductvariations) - Get Product Variants
- [`productCatalogueComCrmProductSelfServiceResourceListProducts`](docs/sdks/productcatalogue/README.md#comcrmproductselfserviceresourcelistproducts) - Search Products
- [`promotionsComCrmPromotionSelfServiceResourceGetSingle`](docs/sdks/promotions/README.md#comcrmpromotionselfserviceresourcegetsingle) - Get Promotion
- [`promotionsComCrmPromotionSelfServiceResourceList`](docs/sdks/promotions/README.md#comcrmpromotionselfserviceresourcelist) - List Promotions
- [`provisioningProvidersComCrmServiceCommandsSelfServiceResourceGetServiceCommands`](docs/sdks/provisioningproviders/README.md#comcrmservicecommandsselfserviceresourcegetservicecommands) - Get Service Commands
- [`provisioningProvidersComCrmServiceCommandsSelfServiceResourceSendServiceCommands`](docs/sdks/provisioningproviders/README.md#comcrmservicecommandsselfserviceresourcesendservicecommands) - Send Service Command
- [`purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions`](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcegetpurchaserewardtransactions) - List Purchase Rewards Breakdown
- [`purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase`](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcegetsinglepurchase) - Get Purchase
- [`purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases`](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcelistpurchases) - Search Contact Purchases
- [`purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase`](docs/sdks/purchasecustomerevents/README.md#comcrmpurchasecustomereventselfserviceresourcereclaimpurchase) - Reclaim Purchase To Contact
- [`recommendationsComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation`](docs/sdks/recommendations/README.md#comcrmorderproductrecommendationselfserviceresourcegetorderproductrecommendation) - Order Product Recommendation Self-Service
- [`recommendationsComCrmProductRecommendationSelfServiceResourceGetProductRecommendation`](docs/sdks/recommendations/README.md#comcrmproductrecommendationselfserviceresourcegetproductrecommendation) - Product Recommendation
- [`recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation`](docs/sdks/recommendations/README.md#comcrmservicerecommendationselfserviceresourcegetservicerecommendation) - Service Recommendation
- [`referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceCreateReferral`](docs/sdks/referralcustomerevents/README.md#comcrmreferralcustomereventselfserviceresourcecreatereferral) - Create Referral
- [`referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceReferralActions`](docs/sdks/referralcustomerevents/README.md#comcrmreferralcustomereventselfserviceresourcereferralactions) - Referral Actions
- [`rewardOffersComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance`](docs/sdks/rewardoffers/README.md#comcrmrewardofferselfserviceresourcegetrewardofferperformance) - Get Reward Offer Performance
- [`rewardOffersComCrmRewardOfferSelfServiceResourceGetSingle`](docs/sdks/rewardoffers/README.md#comcrmrewardofferselfserviceresourcegetsingle) - Get Reward Offer
- [`rewardOffersComCrmRewardOfferSelfServiceResourceList`](docs/sdks/rewardoffers/README.md#comcrmrewardofferselfserviceresourcelist) - Search Reward Offers
- [`rewardSchemesComCrmRewardSchemeSelfServiceResourceList`](docs/sdks/rewardschemes/README.md#comcrmrewardschemeselfserviceresourcelist) - Search Reward Schemes
- [`serviceRequestsComCrmQueueSelfServiceResourceList`](docs/sdks/servicerequests/README.md#comcrmqueueselfserviceresourcelist) - List Service Request Queues
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceCreate`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcecreate) - Create Service Request
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceCreateNote`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcecreatenote) - Create Service Request Note
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceCreateServiceRequestFile`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcecreateservicerequestfile) - Add Service Request Attachment
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceGetFiles`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcegetfiles) - List Service Request Attachments
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceGetNotes`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcegetnotes) - List Service Request Note
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceList`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourcelist) - List Service Requests
- [`serviceRequestsComCrmServiceRequestSelfServiceResourceRemoveFile`](docs/sdks/servicerequests/README.md#comcrmservicerequestselfserviceresourceremovefile) - Delete Service Request Attachment
- [`settingsComCrmNameDayRulesSelfServiceResourceListNameDayRules`](docs/sdks/settings/README.md#comcrmnamedayrulesselfserviceresourcelistnamedayrules) - List Name Day Rules
- [`settingsComCrmProductBrandSelfServiceResourceGetProductBrands`](docs/sdks/settings/README.md#comcrmproductbrandselfserviceresourcegetproductbrands) - List Product Brands
- [`settingsComCrmProductCategorySelfServiceResourceListProductCategories`](docs/sdks/settings/README.md#comcrmproductcategoryselfserviceresourcelistproductcategories) - List Product Categories
- [`settingsComCrmProductTypeSelfServiceResourceListProductTypes`](docs/sdks/settings/README.md#comcrmproducttypeselfserviceresourcelistproducttypes) - List Product Types
- [`subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateBilling`](docs/sdks/subscriptions/README.md#comcrmestimatesubscriptionselfserviceresourceestimatebilling) - Billing
- [`subscriptionsComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscription`](docs/sdks/subscriptions/README.md#comcrmestimatesubscriptionselfserviceresourceestimatesubscription) - Service Delivery
- [`subscriptionsComCrmSubscriptionSelfServiceResourceAddService`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourceaddservice) - Add Service
- [`subscriptionsComCrmSubscriptionSelfServiceResourceChange`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcechange) - Update Subscription
- [`subscriptionsComCrmSubscriptionSelfServiceResourceChangeService`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcechangeservice) - Update Service
- [`subscriptionsComCrmSubscriptionSelfServiceResourceGetSubscriptionAction`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcegetsubscriptionaction) - Get Subscription Action
- [`subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptionActions`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistcontactsubscriptionactions) - List Contact Subscription Actions
- [`subscriptionsComCrmSubscriptionSelfServiceResourceListContactSubscriptions`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistcontactsubscriptions) - List Contact Subscriptions
- [`subscriptionsComCrmSubscriptionSelfServiceResourceListServiceDevices`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistservicedevices) - Get Service Devices
- [`subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionActions`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistsubscriptionactions) - List Subscription Actions
- [`subscriptionsComCrmSubscriptionSelfServiceResourceListSubscriptionServices`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourcelistsubscriptionservices) - List Contact Services
- [`subscriptionsComCrmSubscriptionSelfServiceResourceUpdateSubscriptionAction`](docs/sdks/subscriptions/README.md#comcrmsubscriptionselfserviceresourceupdatesubscriptionaction) - Update Subscription Action
- [`tagsComCrmOrganisationTagSelfServiceResourceListOrganisationTags`](docs/sdks/tags/README.md#comcrmorganisationtagselfserviceresourcelistorganisationtags) - List Organisation Tags
- [`tagsComCrmTagSelfServiceResourceListTags`](docs/sdks/tags/README.md#comcrmtagselfserviceresourcelisttags) - List Tags
- [`usageComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance`](docs/sdks/usage/README.md#comcrmestimateallowanceselfserviceresourceestimatesallowance) - Authorise Usage Consumption
- [`usageComCrmUsageDetailRecordSelfServiceResourceGetMetrics`](docs/sdks/usage/README.md#comcrmusagedetailrecordselfserviceresourcegetmetrics) - Get Usage Records Metrics
- [`usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords`](docs/sdks/usage/README.md#comcrmusagedetailrecordselfserviceresourcelistusagedetailrecords) - List Usage Records
- [`wifiComCrmSelfServiceWifiAuthorizationResourceAuthorizeContact`](docs/sdks/wifi/README.md#comcrmselfservicewifiauthorizationresourceauthorizecontact) - Contact WiFi Authorization
- ~~[`paymentFormsComCrmPaymentFormSelfServiceResourceGenerateAddCardForm`](docs/sdks/paymentforms/README.md#comcrmpaymentformselfserviceresourcegenerateaddcardform)~~ - Add Card :warning: **Deprecated**
- ~~[`paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm`](docs/sdks/paymentforms/README.md#comcrmpaymentformselfserviceresourcegeneratepasspaymentform)~~ - Get Gift Pass Payment Form :warning: **Deprecated**
- ~~[`paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePaymentForm`](docs/sdks/paymentforms/README.md#comcrmpaymentformselfserviceresourcegeneratepaymentform)~~ - Payment Form :warning: **Deprecated**
- ~~[`payoutFormsComCrmPayoutFormSelfServiceResourceGeneratePayoutForm`](docs/sdks/payoutforms/README.md#comcrmpayoutformselfserviceresourcegeneratepayoutform)~~ - Payout Form :warning: **Deprecated**

</details>
<!-- End Standalone functions [standalone-funcs] -->

<!-- Start File uploads [file-upload] -->
## File uploads

Certain SDK methods accept files as part of a multi-part request. It is possible and typically recommended to upload files as a stream rather than reading the entire contents into memory. This avoids excessive memory consumption and potentially crashing with out-of-memory errors when working with very large files. The following example demonstrates how to attach a file stream to a request.

> [!TIP]
>
> Depending on your JavaScript runtime, there are convenient utilities that return a handle to a file without reading the entire contents into memory:
>
> - **Node.js v20+:** Since v20, Node.js comes with a native `openAsBlob` function in [`node:fs`](https://nodejs.org/docs/latest-v20.x/api/fs.html#fsopenasblobpath-options).
> - **Bun:** The native [`Bun.file`](https://bun.sh/docs/api/file-io#reading-files-bun-file) function produces a file handle that can be used for streaming file uploads.
> - **Browsers:** All supported browsers return an instance to a [`File`](https://developer.mozilla.org/en-US/docs/Web/API/File) when reading the value from an `<input type="file">` element.
> - **Node.js v18:** A file stream can be created using the `fileFrom` helper from [`fetch-blob/from.js`](https://www.npmjs.com/package/fetch-blob).

```typescript
import { Crm } from "crm";
import { openAsBlob } from "node:fs";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.platform.comCrmFileSelfServiceResourceUploadFile({
    file: await openAsBlob("example.file"),
    fileEntityType: "ORDERS",
  });

  console.log(result);
}

run();

```
<!-- End File uploads [file-upload] -->

<!-- Start Retries [retries] -->
## Retries

Some of the endpoints in this SDK support retries.  If you use the SDK without any configuration, it will fall back to the default retry strategy provided by the API.  However, the default retry strategy can be overridden on a per-operation basis, or across the entire SDK.

To change the default retry strategy for a single API call, simply provide a retryConfig object to the call:
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAccounts
    .comCrmAccountSelfServiceResourceGetSingle({
      id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    }, {
      retries: {
        strategy: "backoff",
        backoff: {
          initialInterval: 1,
          maxInterval: 50,
          exponent: 1.1,
          maxElapsedTime: 100,
        },
        retryConnectionErrors: false,
      },
    });

  console.log(result);
}

run();

```

If you'd like to override the default retry strategy for all operations that support retries, you can provide a retryConfig at SDK initialization:
```typescript
import { Crm } from "crm";

const crm = new Crm({
  retryConfig: {
    strategy: "backoff",
    backoff: {
      initialInterval: 1,
      maxInterval: 50,
      exponent: 1.1,
      maxElapsedTime: 100,
    },
    retryConnectionErrors: false,
  },
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
<!-- End Retries [retries] -->

<!-- Start Error Handling [errors] -->
## Error Handling

[`CrmError`](./src/models/errors/crm-error.ts) is the base class for all HTTP error responses. It has the following properties:

| Property            | Type       | Description                                            |
| ------------------- | ---------- | ------------------------------------------------------ |
| `error.message`     | `string`   | Error message                                          |
| `error.statusCode`  | `number`   | HTTP response status code eg `404`                     |
| `error.headers`     | `Headers`  | HTTP response headers                                  |
| `error.body`        | `string`   | HTTP body. Can be empty string if no body is returned. |
| `error.rawResponse` | `Response` | Raw HTTP response                                      |

### Example
```typescript
import { Crm } from "crm";
import * as errors from "crm/models/errors";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  try {
    const result = await crm.contactAccounts
      .comCrmAccountSelfServiceResourceGetSingle({
        id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      });

    console.log(result);
  } catch (error) {
    if (error instanceof errors.CrmError) {
      console.log(error.message);
      console.log(error.statusCode);
      console.log(error.body);
      console.log(error.headers);
    }
  }
}

run();

```

### Error Classes
**Primary error:**
* [`CrmError`](./src/models/errors/crm-error.ts): The base class for HTTP error responses.

<details><summary>Less common errors (6)</summary>

<br />

**Network errors:**
* [`ConnectionError`](./src/models/errors/http-client-errors.ts): HTTP client was unable to make a request to a server.
* [`RequestTimeoutError`](./src/models/errors/http-client-errors.ts): HTTP request timed out due to an AbortSignal signal.
* [`RequestAbortedError`](./src/models/errors/http-client-errors.ts): HTTP request was aborted by the client.
* [`InvalidRequestError`](./src/models/errors/http-client-errors.ts): Any input used to create a request is invalid.
* [`UnexpectedClientError`](./src/models/errors/http-client-errors.ts): Unrecognised or unexpected error.


**Inherit from [`CrmError`](./src/models/errors/crm-error.ts)**:
* [`ResponseValidationError`](./src/models/errors/response-validation-error.ts): Type mismatch between the data returned from the server and the structure expected by the SDK. See `error.rawValue` for the raw value and `error.pretty()` for a nicely formatted multi-line string.

</details>
<!-- End Error Handling [errors] -->

<!-- Start Server Selection [server] -->
## Server Selection

### Server Variables

The default server `https://{server}` contains variables and is set to `https://sandboxapi.crm.com` by default. To override default values, the following parameters are available when initializing the SDK client instance:

| Variable | Parameter                     | Supported Values                                                                                               | Default                | Description   |
| -------- | ----------------------------- | -------------------------------------------------------------------------------------------------------------- | ---------------------- | ------------- |
| `server` | `server: models.ServerServer` | - `"sandboxapi.crm.com"`<br/>- `"stagingapi.crm.com"`<br/>- `"sandboxssapi.crm.com"`<br/>- `"sandbox.crm.com"` | `"sandboxapi.crm.com"` | Server option |

#### Example

```typescript
import { Crm } from "crm";

const crm = new Crm({
  serverIdx: 0,
  server: "sandbox.crm.com",
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

### Override Server URL Per-Client

The default server can be overridden globally by passing a URL to the `serverURL: string` optional parameter when initializing the SDK client instance. For example:
```typescript
import { Crm } from "crm";

const crm = new Crm({
  serverURL: "https://sandboxapi.crm.com",
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
<!-- End Server Selection [server] -->

<!-- Start Custom HTTP Client [http-client] -->
## Custom HTTP Client

The TypeScript SDK makes API calls using an `HTTPClient` that wraps the native
[Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). This
client is a thin wrapper around `fetch` and provides the ability to attach hooks
around the request lifecycle that can be used to modify the request or handle
errors and response.

The `HTTPClient` constructor takes an optional `fetcher` argument that can be
used to integrate a third-party HTTP client or when writing tests to mock out
the HTTP client and feed in fixtures.

The following example shows how to:
- route requests through a proxy server using [undici](https://www.npmjs.com/package/undici)'s ProxyAgent
- use the `"beforeRequest"` hook to add a custom header and a timeout to requests
- use the `"requestError"` hook to log errors

```typescript
import { Crm } from "crm";
import { ProxyAgent } from "undici";
import { HTTPClient } from "crm/lib/http";

const dispatcher = new ProxyAgent("http://proxy.example.com:8080");

const httpClient = new HTTPClient({
  // 'fetcher' takes a function that has the same signature as native 'fetch'.
  fetcher: (input, init) =>
    // 'dispatcher' is specific to undici and not part of the standard Fetch API.
    fetch(input, { ...init, dispatcher } as RequestInit),
});

httpClient.addHook("beforeRequest", (request) => {
  const nextRequest = new Request(request, {
    signal: request.signal || AbortSignal.timeout(5000)
  });

  nextRequest.headers.set("x-custom-header", "custom value");

  return nextRequest;
});

httpClient.addHook("requestError", (error, request) => {
  console.group("Request Error");
  console.log("Reason:", `${error}`);
  console.log("Endpoint:", `${request.method} ${request.url}`);
  console.groupEnd();
});

const sdk = new Crm({ httpClient: httpClient });
```
<!-- End Custom HTTP Client [http-client] -->

<!-- Start Debugging [debug] -->
## Debugging

You can setup your SDK to emit debug logs for SDK requests and responses.

You can pass a logger that matches `console`'s interface as an SDK option.

> [!WARNING]
> Beware that debug logging will reveal secrets, like API tokens in headers, in log messages printed to a console or files. It's recommended to use this feature only during local development and not in production.

```typescript
import { Crm } from "crm";

const sdk = new Crm({ debugLogger: console });
```

You can also enable a default debug logger by setting an environment variable `CRM_DEBUG` to true.
<!-- End Debugging [debug] -->

<!-- Placeholder for Future Speakeasy SDK Sections -->

# Development

## Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

## Contributions

While we value open-source contributions to this SDK, this library is generated programmatically. Any manual changes added to internal files will be overwritten on the next generation. 
We look forward to hearing your feedback. Feel free to open a PR or an issue with a proof of concept and we'll do our best to include it in a future release. 

### SDK Created by [Speakeasy](https://www.speakeasy.com/?utm_source=crm&utm_campaign=typescript)
