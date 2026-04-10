
# List 10

*This model accepts additional fields of type array.*

## Structure

`List10`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `locationId` | `?string` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `title` | `?string` | Optional | Title<br><br>**Constraints**: *Maximum Length*: `64` | getTitle(): ?string | setTitle(?string title): void |
| `ccProductTransactionId` | `?string` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCcProductTransactionId(): ?string | setCcProductTransactionId(?string ccProductTransactionId): void |
| `achProductTransactionId` | `?string` | Optional | ACH Product Transaction Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getAchProductTransactionId(): ?string | setAchProductTransactionId(?string achProductTransactionId): void |
| `dueDate` | `?string` | Optional | Due Date, Format: Y-m-d<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getDueDate(): ?string | setDueDate(?string dueDate): void |
| `itemList` | [`?(ItemList[])`](../../doc/models/item-list.md) | Optional | Item List<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `300`, *Unique Items Required* | getItemList(): ?array | setItemList(?array itemList): void |
| `allowOverpayment` | `?bool` | Optional | Allow Overpayment. | getAllowOverpayment(): ?bool | setAllowOverpayment(?bool allowOverpayment): void |
| `bankFundedOnlyOverride` | `?bool` | Optional | Bank Funded Only override | getBankFundedOnlyOverride(): ?bool | setBankFundedOnlyOverride(?bool bankFundedOnlyOverride): void |
| `email` | `?string` | Optional | Email<br><br>**Constraints**: *Maximum Length*: `128` | getEmail(): ?string | setEmail(?string email): void |
| `contactId` | `?string` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getContactId(): ?string | setContactId(?string contactId): void |
| `contactApiId` | `?string` | Optional | Contact API Id<br><br>**Constraints**: *Maximum Length*: `64` | getContactApiId(): ?string | setContactApiId(?string contactApiId): void |
| `quickInvoiceApiId` | `?string` | Optional | Quick Invoice API Id<br><br>**Constraints**: *Maximum Length*: `64` | getQuickInvoiceApiId(): ?string | setQuickInvoiceApiId(?string quickInvoiceApiId): void |
| `customerId` | `?string` | Optional | Customer Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCustomerId(): ?string | setCustomerId(?string customerId): void |
| `expireDate` | `?string` | Optional | Expire Date.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getExpireDate(): ?string | setExpireDate(?string expireDate): void |
| `allowPartialPay` | `?bool` | Optional | Allow partial pay | getAllowPartialPay(): ?bool | setAllowPartialPay(?bool allowPartialPay): void |
| `attachFilesToEmail` | `?bool` | Optional | Attach Files to Email | getAttachFilesToEmail(): ?bool | setAttachFilesToEmail(?bool attachFilesToEmail): void |
| `sendEmail` | `?bool` | Optional | Send Email | getSendEmail(): ?bool | setSendEmail(?bool sendEmail): void |
| `invoiceNumber` | `?string` | Optional | Invoice number<br><br>**Constraints**: *Maximum Length*: `64` | getInvoiceNumber(): ?string | setInvoiceNumber(?string invoiceNumber): void |
| `itemHeader` | `?string` | Optional | Item Header<br><br>**Constraints**: *Maximum Length*: `250` | getItemHeader(): ?string | setItemHeader(?string itemHeader): void |
| `itemFooter` | `?string` | Optional | Item footer<br><br>**Constraints**: *Maximum Length*: `250` | getItemFooter(): ?string | setItemFooter(?string itemFooter): void |
| `amountDue` | `?float` | Optional | Amount Due | getAmountDue(): ?float | setAmountDue(?float amountDue): void |
| `notificationEmail` | `?string` | Optional | Notification email<br><br>**Constraints**: *Maximum Length*: `640` | getNotificationEmail(): ?string | setNotificationEmail(?string notificationEmail): void |
| `statusId` | `?array` | Optional | - | getStatusId(): ?array | setStatusId(?array statusId): void |
| `statusCode` | `?array` | Optional | - | getStatusCode(): ?array | setStatusCode(?array statusCode): void |
| `note` | `?string` | Optional | Note<br><br>**Constraints**: *Maximum Length*: `200` | getNote(): ?string | setNote(?string note): void |
| `notificationDaysBeforeDueDate` | `?int` | Optional | Notification days before due date<br><br>**Constraints**: `>= 0`, `<= 99` | getNotificationDaysBeforeDueDate(): ?int | setNotificationDaysBeforeDueDate(?int notificationDaysBeforeDueDate): void |
| `notificationDaysAfterDueDate` | `?int` | Optional | Notification days after due date<br><br>**Constraints**: `>= 0`, `<= 99` | getNotificationDaysAfterDueDate(): ?int | setNotificationDaysAfterDueDate(?int notificationDaysAfterDueDate): void |
| `notificationOnDueDate` | `?bool` | Optional | Notification on due date | getNotificationOnDueDate(): ?bool | setNotificationOnDueDate(?bool notificationOnDueDate): void |
| `sendTextToPay` | `?bool` | Optional | Send Text To Pay | getSendTextToPay(): ?bool | setSendTextToPay(?bool sendTextToPay): void |
| `files` | [`?(File[])`](../../doc/models/file.md) | Optional | File Information on `expand` | getFiles(): ?array | setFiles(?array files): void |
| `remainingBalance` | `?float` | Optional | Remaining Balance | getRemainingBalance(): ?float | setRemainingBalance(?float remainingBalance): void |
| `singlePaymentMinAmount` | `?int` | Optional | Single Payment Min Amount | getSinglePaymentMinAmount(): ?int | setSinglePaymentMinAmount(?int singlePaymentMinAmount): void |
| `singlePaymentMaxAmount` | `?int` | Optional | Single Payment Max Amount<br><br>**Default**: `999999999` | getSinglePaymentMaxAmount(): ?int | setSinglePaymentMaxAmount(?int singlePaymentMaxAmount): void |
| `cellPhone` | `?string` | Optional | Cell Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getCellPhone(): ?string | setCellPhone(?string cellPhone): void |
| `tags` | [`?(Tag[])`](../../doc/models/tag.md) | Optional | Tag Information on `expand` | getTags(): ?array | setTags(?array tags): void |
| `quickInvoiceC1` | `?string` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getQuickInvoiceC1(): ?string | setQuickInvoiceC1(?string quickInvoiceC1): void |
| `quickInvoiceC2` | `?string` | Optional | Custom field 2 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getQuickInvoiceC2(): ?string | setQuickInvoiceC2(?string quickInvoiceC2): void |
| `quickInvoiceC3` | `?string` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getQuickInvoiceC3(): ?string | setQuickInvoiceC3(?string quickInvoiceC3): void |
| `autoReopen` | `?bool` | Optional | Auto Reopen. If set to true, a void, refund or detachment of a Transaction Payment will cause the QuickInvoice to be opened again | getAutoReopen(): ?bool | setAutoReopen(?bool autoReopen): void |
| `id` | `?string` | Optional | Quick Invoice ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `modifiedTs` | `?int` | Optional | Modified Time Stamp | getModifiedTs(): ?int | setModifiedTs(?int modifiedTs): void |
| `createdUserId` | `?string` | Optional | Created User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCreatedUserId(): ?string | setCreatedUserId(?string createdUserId): void |
| `modifiedUserId` | `?string` | Optional | Modified User Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getModifiedUserId(): ?string | setModifiedUserId(?string modifiedUserId): void |
| `active` | `?bool` | Optional | Active status | getActive(): ?bool | setActive(?bool active): void |
| `paymentStatusId` | `?int` | Optional | Payment Status Id<br><br>**Constraints**: `>= 1`, `<= 3` | getPaymentStatusId(): ?int | setPaymentStatusId(?int paymentStatusId): void |
| `isActive` | `?bool` | Optional | Register is active | getIsActive(): ?bool | setIsActive(?bool isActive): void |
| `quickInvoiceSetting` | [`?QuickInvoiceSetting1`](../../doc/models/quick-invoice-setting-1.md) | Optional | - | getQuickInvoiceSetting(): ?QuickInvoiceSetting1 | setQuickInvoiceSetting(?QuickInvoiceSetting1 quickInvoiceSetting): void |
| `quickInvoiceViews` | [`?(QuickInvoiceView[])`](../../doc/models/quick-invoice-view.md) | Optional | Quick Invoice View Information on `expand` | getQuickInvoiceViews(): ?array | setQuickInvoiceViews(?array quickInvoiceViews): void |
| `location` | [`?Location18`](../../doc/models/location-18.md) | Optional | - | getLocation(): ?Location18 | setLocation(?Location18 location): void |
| `createdUser` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getCreatedUser(): ?User9 | setCreatedUser(?User9 createdUser): void |
| `modifiedUser` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getModifiedUser(): ?User9 | setModifiedUser(?User9 modifiedUser): void |
| `changelogs` | [`?(Changelog[])`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | getChangelogs(): ?array | setChangelogs(?array changelogs): void |
| `contact` | [`?Contact3`](../../doc/models/contact-3.md) | Optional | - | getContact(): ?Contact3 | setContact(?Contact3 contact): void |
| `logEmails` | [`?(LogEmail[])`](../../doc/models/log-email.md) | Optional | Log Email Information on `expand` | getLogEmails(): ?array | setLogEmails(?array logEmails): void |
| `logSms` | [`?LogSms1`](../../doc/models/log-sms-1.md) | Optional | - | getLogSms(): ?LogSms1 | setLogSms(?LogSms1 logSms): void |
| `transactions` | [`?(Transaction[])`](../../doc/models/transaction.md) | Optional | Transaction Information on `expand` | getTransactions(): ?array | setTransactions(?array transactions): void |
| `ccProductTransaction` | [`?ProductTransaction1`](../../doc/models/product-transaction-1.md) | Optional | - | getCcProductTransaction(): ?ProductTransaction1 | setCcProductTransaction(?ProductTransaction1 ccProductTransaction): void |
| `achProductTransaction` | [`?ProductTransaction1`](../../doc/models/product-transaction-1.md) | Optional | - | getAchProductTransaction(): ?ProductTransaction1 | setAchProductTransaction(?ProductTransaction1 achProductTransaction): void |
| `emailBlacklist` | [`?EmailBlacklist1`](../../doc/models/email-blacklist-1.md) | Optional | - | getEmailBlacklist(): ?EmailBlacklist1 | setEmailBlacklist(?EmailBlacklist1 emailBlacklist): void |
| `smsBlacklist` | [`?SmsBlacklist1`](../../doc/models/sms-blacklist-1.md) | Optional | - | getSmsBlacklist(): ?SmsBlacklist1 | setSmsBlacklist(?SmsBlacklist1 smsBlacklist): void |
| `paymentUrl` | `?string` | Optional | Payment Url Information on `expand` | getPaymentUrl(): ?string | setPaymentUrl(?string paymentUrl): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "title": "My terminal",
  "cc_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "ach_product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "due_date": "2021-12-01",
  "allow_overpayment": true,
  "bank_funded_only_override": true,
  "email": "email@domain.com",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_api_id": "contact12345",
  "quick_invoice_api_id": "quickinvoice12345",
  "customer_id": "11e95f8ec39de8fbdb0a4f1a",
  "expire_date": "2021-12-01",
  "allow_partial_pay": true,
  "attach_files_to_email": true,
  "send_email": true,
  "invoice_number": "invoice12345",
  "item_header": "Quick invoice header sample",
  "item_footer": "Thank you",
  "amount_due": 245.36,
  "notification_email": "email@domain.com",
  "note": "some note",
  "notification_days_before_due_date": 3,
  "notification_days_after_due_date": 7,
  "notification_on_due_date": true,
  "send_text_to_pay": true,
  "remaining_balance": 245.36,
  "single_payment_min_amount": 500,
  "single_payment_max_amount": 500000,
  "cell_phone": "3339998822",
  "quick_invoice_c1": "custom-data-1",
  "quick_invoice_c2": "custom-data-2",
  "quick_invoice_c3": "custom-data-3",
  "auto_reopen": true,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "active": true,
  "payment_status_id": 1,
  "is_active": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

