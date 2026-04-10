
# Retry Transaction

Transaction Information on `expand`

*This model accepts additional fields of type array.*

## Structure

`RetryTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `additionalAmounts` | [`?(AdditionalAmount[])`](../../doc/models/additional-amount.md) | Optional | Additional amounts | getAdditionalAmounts(): ?array | setAdditionalAmounts(?array additionalAmounts): void |
| `billingAddress` | [`?BillingAddress2`](../../doc/models/billing-address-2.md) | Optional | - | getBillingAddress(): ?BillingAddress2 | setBillingAddress(?BillingAddress2 billingAddress): void |
| `checkinDate` | `?string` | Optional | Checkin Date - The time difference between checkin_date and checkout_date must be less than or equal to 99 days. NOTE: if checkin_date is in the future, set the advance_deposit to 1<br><br>> Required if merchant industry type is lodging.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getCheckinDate(): ?string | setCheckinDate(?string checkinDate): void |
| `checkoutDate` | `?string` | Optional | Checkout Date - The time difference between checkin_date and checkout_date must be less than or equal to 99 days.<br><br>> Required if merchant industry type is lodging.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getCheckoutDate(): ?string | setCheckoutDate(?string checkoutDate): void |
| `clerkNumber` | `?string` | Optional | Clerk or Employee Identifier<br><br>**Constraints**: *Maximum Length*: `16` | getClerkNumber(): ?string | setClerkNumber(?string clerkNumber): void |
| `contactApiId` | `?string` | Optional | This can be supplied in place of contact_id if you would like to use a contact for the transaction and are using your own custom api_id's to track contacts in the system.<br><br>**Constraints**: *Maximum Length*: `36` | getContactApiId(): ?string | setContactApiId(?string contactApiId): void |
| `contactId` | `?string` | Optional | If contact_id is provided, ensure it belongs to the same location as the transaction. You cannot move transaction across locations.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getContactId(): ?string | setContactId(?string contactId): void |
| `customData` | `?array` | Optional | A field that allows custom JSON to be entered to store extra data. | getCustomData(): ?array | setCustomData(?array customData): void |
| `customerId` | `?string` | Optional | Can be used by Merchants to identify Contacts in our system by an ID from another system.<br><br>**Constraints**: *Maximum Length*: `64` | getCustomerId(): ?string | setCustomerId(?string customerId): void |
| `description` | `?string` | Optional | Description<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64` | getDescription(): ?string | setDescription(?string description): void |
| `identityVerification` | [`?IdentityVerification1`](../../doc/models/identity-verification-1.md) | Optional | - | getIdentityVerification(): ?IdentityVerification1 | setIdentityVerification(?IdentityVerification1 identityVerification): void |
| `iiasInd` | `?array` | Optional | - | getIiasInd(): ?array | setIiasInd(?array iiasInd): void |
| `imageFront` | `?string` | Optional | A base64 encoded string for the image.  Used with Check21 ACH transactions. | getImageFront(): ?string | setImageFront(?string imageFront): void |
| `imageBack` | `?string` | Optional | A base64 encoded string for the image.  Used with Check21 ACH transactions. | getImageBack(): ?string | setImageBack(?string imageBack): void |
| `installment` | `?bool` | Optional | Flag that is allowed to be passed on card not present industries to signify the transaction is a fixed installment plan transaction. | getInstallment(): ?bool | setInstallment(?bool installment): void |
| `installmentNumber` | `?int` | Optional | If this is a fixed installment plan and installment field is being passed as 1, then this field must have a vlue of 1-999 specifying the current installment number that is running.<br><br>**Constraints**: `>= 1`, `<= 999` | getInstallmentNumber(): ?int | setInstallmentNumber(?int installmentNumber): void |
| `installmentCount` | `?int` | Optional | If this is a fixed installment plan and installment field is being passed as 1, then this field must have a vlue of 1-999 specifying the total number of installments on the plan. This number must be grater than or equal to installment_number.<br><br>**Constraints**: `>= 1`, `<= 999` | getInstallmentCount(): ?int | setInstallmentCount(?int installmentCount): void |
| `recurringFlag` | `?array` | Optional | - | getRecurringFlag(): ?array | setRecurringFlag(?array recurringFlag): void |
| `installmentCounter` | `?int` | Optional | Installment Counter<br><br>**Constraints**: `>= 1`, `<= 999` | getInstallmentCounter(): ?int | setInstallmentCounter(?int installmentCounter): void |
| `installmentTotal` | `?int` | Optional | Installment Total<br><br>**Constraints**: `>= 1`, `<= 999` | getInstallmentTotal(): ?int | setInstallmentTotal(?int installmentTotal): void |
| `subscription` | `?bool` | Optional | Subscription | getSubscription(): ?bool | setSubscription(?bool subscription): void |
| `standingOrder` | `?bool` | Optional | Standing Order | getStandingOrder(): ?bool | setStandingOrder(?bool standingOrder): void |
| `locationApiId` | `?string` | Optional | This can be supplied in place of location_id for the transaction if you are using your own custom api_id's for your locations.<br><br>**Constraints**: *Maximum Length*: `36` | getLocationApiId(): ?string | setLocationApiId(?string locationApiId): void |
| `locationId` | `?string` | Optional | A valid Location Id to associate the transaction with.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `productTransactionId` | `?string` | Optional | The Product's method (cc/ach) has to match the action. If not provided, the API will use the default configured for the Location.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getProductTransactionId(): ?string | setProductTransactionId(?string productTransactionId): void |
| `advanceDeposit` | `?bool` | Optional | Advance Deposit | getAdvanceDeposit(): ?bool | setAdvanceDeposit(?bool advanceDeposit): void |
| `noShow` | `?bool` | Optional | Used in Lodging | getNoShow(): ?bool | setNoShow(?bool noShow): void |
| `notificationEmailAddress` | `?string` | Optional | If email is supplied then receipt will be emailed | getNotificationEmailAddress(): ?string | setNotificationEmailAddress(?string notificationEmailAddress): void |
| `orderNumber` | `?string` | Optional | Required for CC transactions , if merchant's deposit account's duplicate check per batch has 'order_number' field<br><br>**Constraints**: *Maximum Length*: `32` | getOrderNumber(): ?string | setOrderNumber(?string orderNumber): void |
| `poNumber` | `?string` | Optional | Purchase Order number<br><br>**Constraints**: *Maximum Length*: `64` | getPoNumber(): ?string | setPoNumber(?string poNumber): void |
| `quickInvoiceId` | `?string` | Optional | Can be used to associate a transaction to a Quick Invoice.  Quick Invoice transactions will have a value for this field automatically.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getQuickInvoiceId(): ?string | setQuickInvoiceId(?string quickInvoiceId): void |
| `recurring` | `?bool` | Optional | Flag that is allowed to be passed on card not present industries to signify the transaction is an ongoing recurring transaction. Possible values to send are 0 or 1. This field must be 0 or not present if installment is sent as 1. | getRecurring(): ?bool | setRecurring(?bool recurring): void |
| `recurringNumber` | `?int` | Optional | If this is an ongoing recurring and recurring field is being passed as 1, then this field must have a vlue of 1-999 specifying the current recurring number that is running.<br><br>**Constraints**: `>= 1`, `<= 999` | getRecurringNumber(): ?int | setRecurringNumber(?int recurringNumber): void |
| `roomNum` | `?string` | Optional | Used in Lodging<br><br>**Constraints**: *Maximum Length*: `12` | getRoomNum(): ?string | setRoomNum(?string roomNum): void |
| `roomRate` | `?int` | Optional | Required if merchant industry type is lodging. | getRoomRate(): ?int | setRoomRate(?int roomRate): void |
| `saveAccount` | `?bool` | Optional | Specifies to save account to contacts profile if account_number/track_data is present with either contact_id or contact_api_id in params. | getSaveAccount(): ?bool | setSaveAccount(?bool saveAccount): void |
| `saveAccountTitle` | `?string` | Optional | If saving token while running a transaction, this will be the title of the token.<br><br>**Constraints**: *Maximum Length*: `16` | getSaveAccountTitle(): ?string | setSaveAccountTitle(?string saveAccountTitle): void |
| `subtotalAmount` | `?int` | Optional | This field is allowed and required for transactions that have a product where surcharge is configured. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getSubtotalAmount(): ?int | setSubtotalAmount(?int subtotalAmount): void |
| `surchargeAmount` | `?int` | Optional | This field is allowed and required for transactions that have a product where surcharge is configured. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getSurchargeAmount(): ?int | setSurchargeAmount(?int surchargeAmount): void |
| `tags` | `?(string[])` | Optional | Tags | getTags(): ?array | setTags(?array tags): void |
| `tax` | `?int` | Optional | Amount of Sales tax - If supplied, this amount should be included in the total transaction_amount field. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getTax(): ?int | setTax(?int tax): void |
| `tipAmount` | `?int` | Optional | Optional tip amount. Tip is not supported for lodging and ecommerce merchants. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getTipAmount(): ?int | setTipAmount(?int tipAmount): void |
| `transactionAmount` | `?int` | Optional | Amount of the transaction. This should always be the desired settle amount of the transaction. Use only integer numbers, so $10.99 will be 1099.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getTransactionAmount(): ?int | setTransactionAmount(?int transactionAmount): void |
| `secondaryAmount` | `?int` | Optional | Retained Amount of the transaction. This should always be less than transaction amount. Use only integer numbers, so $10.99 will be 1099<br><br>**Constraints**: `>= 0`, `<= 999999999` | getSecondaryAmount(): ?int | setSecondaryAmount(?int secondaryAmount): void |
| `transactionApiId` | `?string` | Optional | See api_id page for more details<br><br>**Constraints**: *Maximum Length*: `64` | getTransactionApiId(): ?string | setTransactionApiId(?string transactionApiId): void |
| `transactionC1` | `?string` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getTransactionC1(): ?string | setTransactionC1(?string transactionC1): void |
| `transactionC2` | `?string` | Optional | Custom field 2 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getTransactionC2(): ?string | setTransactionC2(?string transactionC2): void |
| `transactionC3` | `?string` | Optional | Custom field 3 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getTransactionC3(): ?string | setTransactionC3(?string transactionC3): void |
| `bankFundedOnlyOverride` | `?bool` | Optional | Bank Funded Only Override | getBankFundedOnlyOverride(): ?bool | setBankFundedOnlyOverride(?bool bankFundedOnlyOverride): void |
| `allowPartialAuthorizationOverride` | `?bool` | Optional | Allow Partial Authorization Override | getAllowPartialAuthorizationOverride(): ?bool | setAllowPartialAuthorizationOverride(?bool allowPartialAuthorizationOverride): void |
| `autoDeclineCvvOverride` | `?bool` | Optional | Auto Decline CVV Override | getAutoDeclineCvvOverride(): ?bool | setAutoDeclineCvvOverride(?bool autoDeclineCvvOverride): void |
| `autoDeclineStreetOverride` | `?bool` | Optional | Auto Decline Street Override | getAutoDeclineStreetOverride(): ?bool | setAutoDeclineStreetOverride(?bool autoDeclineStreetOverride): void |
| `autoDeclineZipOverride` | `?bool` | Optional | Auto Decline Zip Override | getAutoDeclineZipOverride(): ?bool | setAutoDeclineZipOverride(?bool autoDeclineZipOverride): void |
| `ebtType` | `?array` | Optional | - | getEbtType(): ?array | setEbtType(?array ebtType): void |
| `id` | `?string` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `modifiedTs` | `?int` | Optional | Modified Time Stamp | getModifiedTs(): ?int | setModifiedTs(?int modifiedTs): void |
| `terminalId` | `?string` | Optional | Terminal ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getTerminalId(): ?string | setTerminalId(?string terminalId): void |
| `accountHolderName` | `?string` | Optional | For CC, this is the 'Name (as it appears) on Card'. For ACH, this is the 'Name on Account'.<br><br>> Required for ACH transactions if account_vault_id is not provided. For CC transactions that are run through a terminal, this field may be overwritten by data acquired from the credit card track data.<br><br>**Constraints**: *Maximum Length*: `32` | getAccountHolderName(): ?string | setAccountHolderName(?string accountHolderName): void |
| `accountType` | `?string` | Optional | Required for ACH transactions if account_vault_id is not provided.<br><br>> For ACH, allowed values are 'checking' or 'savings'. For CC, this field is read only. The system will identify card type and generate a value for this field automatically. possible values are: visa, mc, disc, amex, jcb, diners, and debit.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `32` | getAccountType(): ?string | setAccountType(?string accountType): void |
| `tokenApiId` | `?string` | Optional | This can be supplied in place of account_vault_id if you would like to use an token for the transaction and are using your own custom api_id's to track accountvaults in the system.<br><br>**Constraints**: *Maximum Length*: `36` | getTokenApiId(): ?string | setTokenApiId(?string tokenApiId): void |
| `tokenId` | `?string` | Optional | Required if account_number,  track_data, micr_data is not provided.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getTokenId(): ?string | setTokenId(?string tokenId): void |
| `achIdentifier` | `?string` | Optional | Required for ACH transactions in certain scenarios.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `1` | getAchIdentifier(): ?string | setAchIdentifier(?string achIdentifier): void |
| `achSecCode` | `?array` | Optional | - | getAchSecCode(): ?array | setAchSecCode(?array achSecCode): void |
| `authAmount` | `?int` | Optional | Authorization Amount<br><br>**Constraints**: `<= 999999999` | getAuthAmount(): ?int | setAuthAmount(?int authAmount): void |
| `authCode` | `?string` | Optional | Required on force transactions and EBT voucher clear sale/refund. Ignored for all other actions.<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6` | getAuthCode(): ?string | setAuthCode(?string authCode): void |
| `avs` | `?array` | Optional | - | getAvs(): ?array | setAvs(?array avs): void |
| `avsEnhanced` | `?string` | Optional | AVS Enhanced<br><br>**Constraints**: *Minimum Length*: `1` | getAvsEnhanced(): ?string | setAvsEnhanced(?string avsEnhanced): void |
| `cardholderPresent` | `?bool` | Optional | If the cardholder is present at the point of service | getCardholderPresent(): ?bool | setCardholderPresent(?bool cardholderPresent): void |
| `cardPresent` | `?bool` | Optional | A POST only field to specify whether or not the card is present.<br><br>> This field will be defaulted to '1' for all card present industries (retail, lodging, restaurant) and '0' for card not present industries (MOTO/e-commerce).<br>> For lodging, if the no_show flag is set to '1', this field will automatically be set to '0'.<br>> For transactions where account_vault_id is used, this filed will be set to '0'. | getCardPresent(): ?bool | setCardPresent(?bool cardPresent): void |
| `checkNumber` | `?string` | Optional | Required for transactions using TEL SEC code.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `15` | getCheckNumber(): ?string | setCheckNumber(?string checkNumber): void |
| `customerIp` | `?string` | Optional | Can be used to store customer IP Address | getCustomerIp(): ?string | setCustomerIp(?string customerIp): void |
| `cvvResponse` | `?string` | Optional | Obfuscated CVV<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `1` | getCvvResponse(): ?string | setCvvResponse(?string cvvResponse): void |
| `entryModeId` | `?array` | Optional | - | getEntryModeId(): ?array | setEntryModeId(?array entryModeId): void |
| `emvReceiptData` | `?array` | Optional | - | getEmvReceiptData(): ?array | setEmvReceiptData(?array emvReceiptData): void |
| `firstSix` | `?string` | Optional | First six numbers of account_number.  Automatically generated by system.<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6` | getFirstSix(): ?string | setFirstSix(?string firstSix): void |
| `lastFour` | `?string` | Optional | Last four numbers of account_number.  Automatically generated by the system.<br><br>**Constraints**: *Minimum Length*: `4`, *Maximum Length*: `4` | getLastFour(): ?string | setLastFour(?string lastFour): void |
| `paymentMethod` | [`?string(PaymentMethod9)`](../../doc/models/payment-method-9.md) | Optional | - | getPaymentMethod(): ?string | setPaymentMethod(?string paymentMethod): void |
| `terminalSerialNumber` | `?string` | Optional | If transaction was processed using a terminal, this field would contain the terminal's serial number<br><br>**Constraints**: *Maximum Length*: `36`, *Pattern*: `^[a-zA-Z0-9]*$` | getTerminalSerialNumber(): ?string | setTerminalSerialNumber(?string terminalSerialNumber): void |
| `transactionSettlementStatus` | `?string` | Optional | (Deprecated field)<br><br>**Constraints**: *Maximum Length*: `32` | getTransactionSettlementStatus(): ?string | setTransactionSettlementStatus(?string transactionSettlementStatus): void |
| `chargeBackDate` | `?string` | Optional | Charge Back Date (ACH Trxs)<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getChargeBackDate(): ?string | setChargeBackDate(?string chargeBackDate): void |
| `isRecurring` | `?bool` | Optional | Flag that is allowed to be passed on card not present industries to signify the transaction is a fixed installment plan transaction. | getIsRecurring(): ?bool | setIsRecurring(?bool isRecurring): void |
| `notificationEmailSent` | `?bool` | Optional | Indicates if email receipt has been sent | getNotificationEmailSent(): ?bool | setNotificationEmailSent(?bool notificationEmailSent): void |
| `par` | `?string` | Optional | A field usually returned form the processor to uniquely identifier a specific cardholder's credit card.<br><br>**Constraints**: *Maximum Length*: `36` | getPar(): ?string | setPar(?string par): void |
| `reasonCodeId` | `?array` | Optional | - | getReasonCodeId(): ?array | setReasonCodeId(?array reasonCodeId): void |
| `recurringId` | `?string` | Optional | A unique identifer used to associate a transaction with a Recurring.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getRecurringId(): ?string | setRecurringId(?string recurringId): void |
| `settleDate` | `?string` | Optional | Settle date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getSettleDate(): ?string | setSettleDate(?string settleDate): void |
| `statusCode` | `?array` | Optional | - | getStatusCode(): ?array | setStatusCode(?array statusCode): void |
| `transactionBatchId` | `?string` | Optional | For cc transactions, this is the id of the batch the transaction belongs to (not to be confused with batch number). This will be null for transactions that do not settle (void and authonly).<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getTransactionBatchId(): ?string | setTransactionBatchId(?string transactionBatchId): void |
| `typeId` | `?array` | Optional | - | getTypeId(): ?array | setTypeId(?array typeId): void |
| `verbiage` | `?string` | Optional | Verbiage -Do not use verbiage to see if the transaction was approved, use status_id | getVerbiage(): ?string | setVerbiage(?string verbiage): void |
| `voucherNumber` | `?string` | Optional | Voucher Number | getVoucherNumber(): ?string | setVoucherNumber(?string voucherNumber): void |
| `voidDate` | `?string` | Optional | void date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getVoidDate(): ?string | setVoidDate(?string voidDate): void |
| `batch` | `?string` | Optional | Batch | getBatch(): ?string | setBatch(?string batch): void |
| `termsAgree` | `?bool` | Optional | Terms Agreement | getTermsAgree(): ?bool | setTermsAgree(?bool termsAgree): void |
| `responseMessage` | `?string` | Optional | Response Message<br><br>**Constraints**: *Maximum Length*: `255` | getResponseMessage(): ?string | setResponseMessage(?string responseMessage): void |
| `returnDate` | `?string` | Optional | Return Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getReturnDate(): ?string | setReturnDate(?string returnDate): void |
| `trxSourceId` | `?array` | Optional | - | getTrxSourceId(): ?array | setTrxSourceId(?array trxSourceId): void |
| `routingNumber` | `?string` | Optional | This field is read only for ach on transactions. Must be supplied if account_vault_id is not provided. | getRoutingNumber(): ?string | setRoutingNumber(?string routingNumber): void |
| `trxSourceCode` | `?array` | Optional | - | getTrxSourceCode(): ?array | setTrxSourceCode(?array trxSourceCode): void |
| `paylinkId` | `?string` | Optional | Paylink Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getPaylinkId(): ?string | setPaylinkId(?string paylinkId): void |
| `currencyCode` | `?float` | Optional | Currency Code<br><br>**Default**: `840` | getCurrencyCode(): ?float | setCurrencyCode(?float currencyCode): void |
| `isAccountvault` | `?bool` | Optional | Is Token Transaction | getIsAccountvault(): ?bool | setIsAccountvault(?bool isAccountvault): void |
| `createdUserId` | `?string` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCreatedUserId(): ?string | setCreatedUserId(?string createdUserId): void |
| `modifiedUserId` | `?string` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getModifiedUserId(): ?string | setModifiedUserId(?string modifiedUserId): void |
| `transactionCode` | `?string` | Optional | Transaction Code | getTransactionCode(): ?string | setTransactionCode(?string transactionCode): void |
| `effectiveDate` | `?string` | Optional | For ACH only, this is optional and defaults to current day.<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getEffectiveDate(): ?string | setEffectiveDate(?string effectiveDate): void |
| `notificationPhone` | `?string` | Optional | Notification Phone. Country code not included | getNotificationPhone(): ?string | setNotificationPhone(?string notificationPhone): void |
| `cavvResult` | `?string` | Optional | Cavv Result | getCavvResult(): ?string | setCavvResult(?string cavvResult): void |
| `isToken` | `?bool` | Optional | Is Token Transaction | getIsToken(): ?bool | setIsToken(?bool isToken): void |
| `accountVaultId` | `?string` | Optional | Token ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getAccountVaultId(): ?string | setAccountVaultId(?string accountVaultId): void |
| `hostedPaymentPageId` | `?string` | Optional | Hosted Payment Page Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getHostedPaymentPageId(): ?string | setHostedPaymentPageId(?string hostedPaymentPageId): void |
| `stan` | `?string` | Optional | - | getStan(): ?string | setStan(?string stan): void |
| `currency` | `?string` | Optional | Currency | getCurrency(): ?string | setCurrency(?string currency): void |
| `cardBin` | `?string` | Optional | Card Bin | getCardBin(): ?string | setCardBin(?string cardBin): void |
| `walletType` | `?string` | Optional | This value provides information from where the transaction was initialized (Such as In-App provider) | getWalletType(): ?string | setWalletType(?string walletType): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "checkin_date": "2021-12-01",
  "checkout_date": "2021-12-01",
  "clerk_number": "AE1234",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "custom_data": {
    "data1": "custom1",
    "data2": "custom2"
  },
  "customer_id": "customerid",
  "description": "some description",
  "image_front": "U29tZVN0cmluZ09idmlvdXNseU5vdEJhc2U2NEVuY29kZWQ=",
  "image_back": "U29tZVN0cmluZ09idmlvdXNseU5vdEJhc2U2NEVuY29kZWQ=",
  "installment": true,
  "installment_number": 1,
  "installment_count": 1,
  "installment_counter": 1,
  "installment_total": 1,
  "subscription": false,
  "standing_order": false,
  "location_api_id": "location-api-id-florida-2",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "advance_deposit": false,
  "no_show": false,
  "notification_email_address": "johnsmith@smiths.com",
  "order_number": "433659378839",
  "po_number": "555555553123",
  "quick_invoice_id": "11e95f8ec39de8fbdb0a4f1a",
  "recurring": false,
  "recurring_number": 1,
  "room_num": "303",
  "room_rate": 95,
  "save_account": false,
  "save_account_title": "John Account",
  "subtotal_amount": 599,
  "surcharge_amount": 100,
  "tax": 0,
  "tip_amount": 0,
  "transaction_amount": 0,
  "secondary_amount": 0,
  "transaction_api_id": "transaction-payment-abcd123",
  "transaction_c1": "custom-data-1",
  "transaction_c2": "custom-data-2",
  "transaction_c3": "custom-data-3",
  "bank_funded_only_override": false,
  "allow_partial_authorization_override": false,
  "auto_decline_cvv_override": false,
  "auto_decline_street_override": false,
  "auto_decline_zip_override": false,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "terminal_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_holder_name": "smith",
  "account_type": "checking",
  "token_id": "11e95f8ec39de8fbdb0a4f1a",
  "ach_identifier": "P",
  "auth_amount": 1,
  "auth_code": "BR349K",
  "avs_enhanced": "N",
  "cardholder_present": true,
  "card_present": true,
  "check_number": "8520748520963",
  "customer_ip": "192.168.0.10",
  "cvv_response": "N",
  "first_six": "545454",
  "last_four": "5454",
  "terminal_serial_number": "1234567890",
  "charge_back_date": "2021-12-01",
  "is_recurring": true,
  "notification_email_sent": true,
  "par": "Q1J4Z28RKA1EBL470G9XYG90R5D3E",
  "recurring_id": "11e95f8ec39de8fbdb0a4f1a",
  "settle_date": "2021-12-01",
  "transaction_batch_id": "11e95f8ec39de8fbdb0a4f1a",
  "verbiage": "APPROVED",
  "voucher_number": "1234",
  "void_date": "2021-12-01",
  "batch": "2",
  "terms_agree": true,
  "return_date": "2021-12-01",
  "routing_number": "051904524",
  "paylink_id": "11e95f8ec39de8fbdb0a4f1a",
  "currency_code": 840,
  "is_accountvault": true,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "effective_date": "2021-12-01",
  "is_token": true,
  "account_vault_id": "11e95f8ec39de8fbdb0a4f1a",
  "hosted_payment_page_id": "11e95f8ec39de8fbdb0a4f1a",
  "additional_amounts": [
    {
      "type": {
        "key1": "val1",
        "key2": "val2"
      },
      "amount": 6,
      "account_type": {
        "key1": "val1",
        "key2": "val2"
      },
      "currency": 154.64,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "billing_address": {
    "city": "city2",
    "state": "state6",
    "postal_code": "postal_code0",
    "street": "street8",
    "phone": "phone2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

