
# V1 Paylinks Request 1

*This model accepts additional fields of type array.*

## Structure

`V1PaylinksRequest1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `locationId` | `?string` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `ccProductTransactionId` | `?string` | Optional | cc_product_transaction_id that has paylinks enabled in the service settings.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCcProductTransactionId(): ?string | setCcProductTransactionId(?string ccProductTransactionId): void |
| `email` | `?string` | Optional | Optional. An email address that should be used as the "To" address when sending a Paylink Notification email.<br><br>**Constraints**: *Maximum Length*: `128` | getEmail(): ?string | setEmail(?string email): void |
| `amountDue` | `?int` | Optional | This is the amount that need to be paid (automatically calculated by system). amount_due= sum of items in item_list<br><br>**Constraints**: `>= 1`, `<= 999999999` | getAmountDue(): ?int | setAmountDue(?int amountDue): void |
| `locationApiId` | `?string` | Optional | Location Api Id. System id | getLocationApiId(): ?string | setLocationApiId(?string locationApiId): void |
| `contactId` | `?string` | Optional | Include the Contact_id that the Paylink will belong to. This will allow you to query the List All Paylinks and filter_by Contact_id to see the status of all the contacts Paylinks.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getContactId(): ?string | setContactId(?string contactId): void |
| `contactApiId` | `?string` | Optional | Integrator provided unique id that was provided during the contact creation for the Fortis Contact. Include the Contact_id that the Paylink will belong to. This will allow you to query the List All Paylinks and filter_by Contact_id to see the status of all the contacts Paylinks. | getContactApiId(): ?string | setContactApiId(?string contactApiId): void |
| `paylinkApiId` | `?string` | Optional | Integrator provided id that prevents duplicate Paylinke Api Id's per location.<br><br>**Constraints**: *Maximum Length*: `64` | getPaylinkApiId(): ?string | setPaylinkApiId(?string paylinkApiId): void |
| `achProductTransactionId` | `?string` | Optional | ACH product transaction on which Paylink is created. This field is optional and will default to default_ach product if not supplied at all. Either this or cc_product_transaction_id must be supplied. Changes are allowed on PUT if payments have not been made against Paylink.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getAchProductTransactionId(): ?string | setAchProductTransactionId(?string achProductTransactionId): void |
| `expireDate` | `?string` | Optional | Expire Date of Paylink. Optional<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getExpireDate(): ?string | setExpireDate(?string expireDate): void |
| `displayProductTransactionReceiptDetails` | `?bool` | Optional | Display Product Transaction Receipt Details. Show the receipt details after the successful payment | getDisplayProductTransactionReceiptDetails(): ?bool | setDisplayProductTransactionReceiptDetails(?bool displayProductTransactionReceiptDetails): void |
| `displayBillingFields` | `?bool` | Optional | Display Billing Fields to show the billing field inputs in the paylink form | getDisplayBillingFields(): ?bool | setDisplayBillingFields(?bool displayBillingFields): void |
| `deliveryMethod` | `?array` | Optional | - | getDeliveryMethod(): ?array | setDeliveryMethod(?array deliveryMethod): void |
| `cellPhone` | `?string` | Optional | Required if delivery_method is set to 2[SMS], 3[Both email and sms], this will be the recipient of the SMS<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{1,10}$` | getCellPhone(): ?string | setCellPhone(?string cellPhone): void |
| `description` | `?string` | Optional | Add a Description for reporting purposes<br><br>**Constraints**: *Maximum Length*: `64` | getDescription(): ?string | setDescription(?string description): void |
| `storeToken` | `?bool` | Optional | Store Token to create a token_id(account_vault_id) to be used for future payment types(CC Sale Tokenized, ACH Debit Tokenized) | getStoreToken(): ?bool | setStoreToken(?bool storeToken): void |
| `storeTokenTitle` | `?string` | Optional | Store Token Title can be used to set the name of the token, sucha John Smith<br><br>**Constraints**: *Maximum Length*: `16` | getStoreTokenTitle(): ?string | setStoreTokenTitle(?string storeTokenTitle): void |
| `paylinkAction` | `?array` | Optional | - | getPaylinkAction(): ?array | setPaylinkAction(?array paylinkAction): void |
| `bankFundedOnlyOverride` | `?bool` | Optional | Bank Funded Only Override | getBankFundedOnlyOverride(): ?bool | setBankFundedOnlyOverride(?bool bankFundedOnlyOverride): void |
| `tags` | `?(string[])` | Optional | Used to apply tags to a paylink. | getTags(): ?array | setTags(?array tags): void |
| `redirectUrlDelay` | `?float` | Optional | Redirect URL Delay in seconds<br><br>**Constraints**: `<= 15` | getRedirectUrlDelay(): ?float | setRedirectUrlDelay(?float redirectUrlDelay): void |
| `redirectUrlOnApprove` | `?string` | Optional | Redirect URL On Approved transactions | getRedirectUrlOnApprove(): ?string | setRedirectUrlOnApprove(?string redirectUrlOnApprove): void |
| `redirectUrlOnDecline` | `?string` | Optional | Redirect URL On Declined transactions | getRedirectUrlOnDecline(): ?string | setRedirectUrlOnDecline(?string redirectUrlOnDecline): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "email": "email@domain.com",
  "amount_due": 1,
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "expire_date": "2021-12-01",
  "display_product_transaction_receipt_details": true,
  "display_billing_fields": true,
  "cell_phone": "3339998822",
  "description": "Description",
  "store_token": false,
  "store_token_title": "John Account",
  "bank_funded_only_override": false,
  "redirect_url_delay": 15,
  "location_api_id": "location_api_id4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

