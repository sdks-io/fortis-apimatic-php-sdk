
# List 1

*This model accepts additional fields of type array.*

## Structure

`List1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `locationId` | `?string` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `accountNumber` | `?string` | Optional | Contact Account Number<br><br>**Constraints**: *Maximum Length*: `32` | getAccountNumber(): ?string | setAccountNumber(?string accountNumber): void |
| `contactApiId` | `?string` | Optional | Contact API Id<br><br>**Constraints**: *Maximum Length*: `64`, *Pattern*: `^[a-zA-Z0-9]*$` | getContactApiId(): ?string | setContactApiId(?string contactApiId): void |
| `firstName` | `?string` | Optional | First Name<br><br>**Constraints**: *Maximum Length*: `64` | getFirstName(): ?string | setFirstName(?string firstName): void |
| `lastName` | `?string` | Optional | Last Name<br><br>**Constraints**: *Maximum Length*: `64` | getLastName(): ?string | setLastName(?string lastName): void |
| `cellPhone` | `?string` | Optional | Cell phone of contact<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getCellPhone(): ?string | setCellPhone(?string cellPhone): void |
| `balance` | `?float` | Optional | Balance<br><br>**Constraints**: `>= -99999999.99`, `<= 99999999.99` | getBalance(): ?float | setBalance(?float balance): void |
| `address` | [`?Address4`](../../doc/models/address-4.md) | Optional | - | getAddress(): ?Address4 | setAddress(?Address4 address): void |
| `companyName` | `?string` | Optional | Company Name<br><br>**Constraints**: *Maximum Length*: `64` | getCompanyName(): ?string | setCompanyName(?string companyName): void |
| `headerMessage` | `?string` | Optional | Header Message<br><br>**Constraints**: *Maximum Length*: `250` | getHeaderMessage(): ?string | setHeaderMessage(?string headerMessage): void |
| `dateOfBirth` | `?string` | Optional | Contacts DOB, Format: yyyy-MM-dd<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getDateOfBirth(): ?string | setDateOfBirth(?string dateOfBirth): void |
| `emailTrxReceipt` | `?bool` | Optional | Whether or not to email all transactions receipts to contact (1 or 0) | getEmailTrxReceipt(): ?bool | setEmailTrxReceipt(?bool emailTrxReceipt): void |
| `homePhone` | `?string` | Optional | Contacts home phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getHomePhone(): ?string | setHomePhone(?string homePhone): void |
| `officePhone` | `?string` | Optional | Contacts office phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getOfficePhone(): ?string | setOfficePhone(?string officePhone): void |
| `officePhoneExt` | `?string` | Optional | Contacts office phone extension for office phone<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^\d{1,10}$` | getOfficePhoneExt(): ?string | setOfficePhoneExt(?string officePhoneExt): void |
| `homePhoneCountryCode` | `?string` | Optional | Home phone country code<br><br>**Constraints**: *Maximum Length*: `6`, *Pattern*: `^\+([\d]+)$` | getHomePhoneCountryCode(): ?string | setHomePhoneCountryCode(?string homePhoneCountryCode): void |
| `officePhoneCountryCode` | `?string` | Optional | Office phone country code<br><br>**Constraints**: *Maximum Length*: `6`, *Pattern*: `^\+([\d]+)$` | getOfficePhoneCountryCode(): ?string | setOfficePhoneCountryCode(?string officePhoneCountryCode): void |
| `cellPhoneCountryCode` | `?string` | Optional | Cell phone country code<br><br>**Constraints**: *Maximum Length*: `6`, *Pattern*: `^\+([\d]+)$` | getCellPhoneCountryCode(): ?string | setCellPhoneCountryCode(?string cellPhoneCountryCode): void |
| `headerMessageType` | `?int` | Optional | Header Message Type<br><br>**Constraints**: `>= 0`, `<= 4` | getHeaderMessageType(): ?int | setHeaderMessageType(?int headerMessageType): void |
| `updateIfExists` | `?array` | Optional | - | getUpdateIfExists(): ?array | setUpdateIfExists(?array updateIfExists): void |
| `contactC1` | `?string` | Optional | Custom field 1 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getContactC1(): ?string | setContactC1(?string contactC1): void |
| `contactC2` | `?string` | Optional | Custom field 2 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getContactC2(): ?string | setContactC2(?string contactC2): void |
| `contactC3` | `?string` | Optional | Custom field 3 for api users to store custom data<br><br>**Constraints**: *Maximum Length*: `128` | getContactC3(): ?string | setContactC3(?string contactC3): void |
| `parentId` | `?string` | Optional | Parent Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getParentId(): ?string | setParentId(?string parentId): void |
| `email` | `?string` | Optional | Email of contact<br><br>**Constraints**: *Maximum Length*: `64` | getEmail(): ?string | setEmail(?string email): void |
| `tokenImportId` | `?string` | Optional | Token Import Id<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getTokenImportId(): ?string | setTokenImportId(?string tokenImportId): void |
| `id` | `?string` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `modifiedTs` | `?int` | Optional | Modified Time Stamp | getModifiedTs(): ?int | setModifiedTs(?int modifiedTs): void |
| `active` | `?bool` | Optional | Active | getActive(): ?bool | setActive(?bool active): void |
| `createdUserId` | `?string` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCreatedUserId(): ?string | setCreatedUserId(?string createdUserId): void |
| `receivedEmails` | [`?(ReceivedEmail[])`](../../doc/models/received-email.md) | Optional | Received Email Information on `expand` | getReceivedEmails(): ?array | setReceivedEmails(?array receivedEmails): void |
| `isDeletable` | `?bool` | Optional | Is Deletable Information on `expand` | getIsDeletable(): ?bool | setIsDeletable(?bool isDeletable): void |
| `location` | [`?Location18`](../../doc/models/location-18.md) | Optional | - | getLocation(): ?Location18 | setLocation(?Location18 location): void |
| `user` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getUser(): ?User9 | setUser(?User9 user): void |
| `recurrings` | [`?(Recurring[])`](../../doc/models/recurring.md) | Optional | Recurring Information on `expand` | getRecurrings(): ?array | setRecurrings(?array recurrings): void |
| `emailBlacklist` | [`?EmailBlacklist1`](../../doc/models/email-blacklist-1.md) | Optional | - | getEmailBlacklist(): ?EmailBlacklist1 | setEmailBlacklist(?EmailBlacklist1 emailBlacklist): void |
| `smsBlacklist` | [`?SmsBlacklist1`](../../doc/models/sms-blacklist-1.md) | Optional | - | getSmsBlacklist(): ?SmsBlacklist1 | setSmsBlacklist(?SmsBlacklist1 smsBlacklist): void |
| `changelogs` | [`?(Changelog[])`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | getChangelogs(): ?array | setChangelogs(?array changelogs): void |
| `postbackLogs` | [`?(PostbackLog[])`](../../doc/models/postback-log.md) | Optional | Postback Log Information on `expand` | getPostbackLogs(): ?array | setPostbackLogs(?array postbackLogs): void |
| `createdUser` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getCreatedUser(): ?User9 | setCreatedUser(?User9 createdUser): void |
| `parent` | [`?Parent5`](../../doc/models/parent-5.md) | Optional | - | getParent(): ?Parent5 | setParent(?Parent5 parent): void |
| `children` | [`?Children1`](../../doc/models/children-1.md) | Optional | - | getChildren(): ?Children1 | setChildren(?Children1 children): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "account_number": "54545433332",
  "contact_api_id": "137",
  "first_name": "John",
  "last_name": "Smith",
  "cell_phone": "3339998822",
  "balance": 245.36,
  "company_name": "Fortis Payment Systems, LLC",
  "header_message": "This is a sample message for you",
  "date_of_birth": "2021-12-01",
  "email_trx_receipt": true,
  "home_phone": "3339998822",
  "office_phone": "3339998822",
  "office_phone_ext": "5",
  "home_phone_country_code": "+1",
  "office_phone_country_code": "+1",
  "cell_phone_country_code": "+1",
  "header_message_type": 0,
  "contact_c1": "any",
  "contact_c2": "anything",
  "contact_c3": "something",
  "parent_id": "11e95f8ec39de8fbdb0a4f1a",
  "email": "email@domain.com",
  "token_import_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "active": true,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "is_deletable": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

