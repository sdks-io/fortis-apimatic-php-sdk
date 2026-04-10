
# Data 34

*This model accepts additional fields of type array.*

## Structure

`Data34`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `accountNumber` | `?string` | Optional | Account Number | getAccountNumber(): ?string | setAccountNumber(?string accountNumber): void |
| `brandingDomainUrl` | `?string` | Optional | Branding Domain Url<br><br>**Constraints**: *Maximum Length*: `64` | getBrandingDomainUrl(): ?string | setBrandingDomainUrl(?string brandingDomainUrl): void |
| `cellPhone` | `?string` | Optional | Cell Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getCellPhone(): ?string | setCellPhone(?string cellPhone): void |
| `companyName` | `?string` | Optional | Company Name<br><br>**Constraints**: *Maximum Length*: `64` | getCompanyName(): ?string | setCompanyName(?string companyName): void |
| `contactId` | `?string` | Optional | Contact Id Information on `expand` | getContactId(): ?string | setContactId(?string contactId): void |
| `dateOfBirth` | `?string` | Optional | Date Of Birth<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` | getDateOfBirth(): ?string | setDateOfBirth(?string dateOfBirth): void |
| `domainId` | `?string` | Optional | Domain<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getDomainId(): ?string | setDomainId(?string domainId): void |
| `email` | `?string` | Optional | Email<br><br>**Constraints**: *Maximum Length*: `128` | getEmail(): ?string | setEmail(?string email): void |
| `emailTrxReceipt` | `?bool` | Optional | Email Trx Receipt | getEmailTrxReceipt(): ?bool | setEmailTrxReceipt(?bool emailTrxReceipt): void |
| `homePhone` | `?string` | Optional | Home Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getHomePhone(): ?string | setHomePhone(?string homePhone): void |
| `firstName` | `?string` | Optional | First Name<br><br>**Constraints**: *Maximum Length*: `64` | getFirstName(): ?string | setFirstName(?string firstName): void |
| `lastName` | `?string` | Optional | Last Name<br><br>**Constraints**: *Maximum Length*: `64` | getLastName(): ?string | setLastName(?string lastName): void |
| `locale` | `?string` | Optional | Locale<br><br>**Constraints**: *Maximum Length*: `8` | getLocale(): ?string | setLocale(?string locale): void |
| `officePhone` | `?string` | Optional | Office Phone<br><br>**Constraints**: *Minimum Length*: `10`, *Maximum Length*: `10`, *Pattern*: `^\d{10}$` | getOfficePhone(): ?string | setOfficePhone(?string officePhone): void |
| `officeExtPhone` | `?string` | Optional | Office Ext Phone<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^\d{1,10}$` | getOfficeExtPhone(): ?string | setOfficeExtPhone(?string officeExtPhone): void |
| `primaryLocationId` | `?string` | Optional | Primary Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getPrimaryLocationId(): ?string | setPrimaryLocationId(?string primaryLocationId): void |
| `requiresNewPassword` | `?string` | Optional | Requires New Password<br><br>**Constraints**: *Maximum Length*: `1` | getRequiresNewPassword(): ?string | setRequiresNewPassword(?string requiresNewPassword): void |
| `termsConditionCode` | `?string` | Optional | Terms Condition (This field is required when updating your own password). | getTermsConditionCode(): ?string | setTermsConditionCode(?string termsConditionCode): void |
| `tz` | `?string` | Optional | Time zone<br><br>**Constraints**: *Maximum Length*: `30` | getTz(): ?string | setTz(?string tz): void |
| `uiPrefs` | [`?UiPrefs1`](../../doc/models/ui-prefs-1.md) | Optional | - | getUiPrefs(): ?UiPrefs1 | setUiPrefs(?UiPrefs1 uiPrefs): void |
| `username` | `?string` | Optional | Username<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `64` | getUsername(): ?string | setUsername(?string username): void |
| `userApiKey` | `?string` | Optional | User Api Key<br><br>**Constraints**: *Minimum Length*: `16`, *Maximum Length*: `64` | getUserApiKey(): ?string | setUserApiKey(?string userApiKey): void |
| `userHashKey` | `?string` | Optional | User Hash Key<br><br>**Constraints**: *Minimum Length*: `24`, *Maximum Length*: `36` | getUserHashKey(): ?string | setUserHashKey(?string userHashKey): void |
| `userTypeCode` | [`?int(UserTypeCode)`](../../doc/models/user-type-code.md) | Optional | - | getUserTypeCode(): ?int | setUserTypeCode(?int userTypeCode): void |
| `password` | `?string` | Optional | Password<br><br>**Constraints**: *Minimum Length*: `8`, *Maximum Length*: `128`, *Pattern*: ``^(?=.*[`!@#$%^&*()_+\-=\[\]{};':"\\\|,.<>\/?~])(?=.*[0-9])(?=.*[a-zA-Z]).*$`` | getPassword(): ?string | setPassword(?string password): void |
| `zip` | `?string` | Optional | Zip<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `10`, *Pattern*: `^[a-zA-Z0-9\-\s]+$` | getZip(): ?string | setZip(?string zip): void |
| `locationId` | `?string` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `contactApiId` | `?string` | Optional | ContactApi Id | getContactApiId(): ?string | setContactApiId(?string contactApiId): void |
| `primaryLocationApiId` | `?string` | Optional | Primary LocationApi ID | getPrimaryLocationApiId(): ?string | setPrimaryLocationApiId(?string primaryLocationApiId): void |
| `statusCode` | `?array` | Optional | - | getStatusCode(): ?array | setStatusCode(?array statusCode): void |
| `apiOnly` | `?bool` | Optional | API Only | getApiOnly(): ?bool | setApiOnly(?bool apiOnly): void |
| `isInvitation` | `?bool` | Optional | Is Invitation | getIsInvitation(): ?bool | setIsInvitation(?bool isInvitation): void |
| `address` | [`?Address3`](../../doc/models/address-3.md) | Optional | - | getAddress(): ?Address3 | setAddress(?Address3 address): void |
| `id` | `?string` | Optional | User ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `status` | `?bool` | Optional | Status | getStatus(): ?bool | setStatus(?bool status): void |
| `loginAttempts` | `?int` | Optional | Login Attempts | getLoginAttempts(): ?int | setLoginAttempts(?int loginAttempts): void |
| `lastLoginTs` | `?int` | Optional | Last Login | getLastLoginTs(): ?int | setLastLoginTs(?int lastLoginTs): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `modifiedTs` | `?int` | Optional | Modified Time Stamp | getModifiedTs(): ?int | setModifiedTs(?int modifiedTs): void |
| `createdUserId` | `?string` | Optional | Created User<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCreatedUserId(): ?string | setCreatedUserId(?string createdUserId): void |
| `termsAcceptedTs` | `?int` | Optional | Terms Accepted | getTermsAcceptedTs(): ?int | setTermsAcceptedTs(?int termsAcceptedTs): void |
| `termsAgreeIp` | `?string` | Optional | Terms Agree Ip<br><br>**Constraints**: *Maximum Length*: `16` | getTermsAgreeIp(): ?string | setTermsAgreeIp(?string termsAgreeIp): void |
| `currentDateTime` | `?string` | Optional | Current Date Time<br><br>**Constraints**: *Maximum Length*: `24` | getCurrentDateTime(): ?string | setCurrentDateTime(?string currentDateTime): void |
| `currentLoginIp` | `?string` | Optional | Current Login Ip | getCurrentLoginIp(): ?string | setCurrentLoginIp(?string currentLoginIp): void |
| `currentLogin` | `?int` | Optional | Current Login Timestamp | getCurrentLogin(): ?int | setCurrentLogin(?int currentLogin): void |
| `sftpAccess` | `?bool` | Optional | SFTP Access | getSftpAccess(): ?bool | setSftpAccess(?bool sftpAccess): void |
| `logApiResponseBodyTs` | `?int` | Optional | Log Api Response Body | getLogApiResponseBodyTs(): ?int | setLogApiResponseBodyTs(?int logApiResponseBodyTs): void |
| `locations` | [`?(Location18[])`](../../doc/models/location-18.md) | Optional | Location Information on `expand` | getLocations(): ?array | setLocations(?array locations): void |
| `primaryLocation` | [`?AccountVaultCauProductTransaction`](../../doc/models/account-vault-cau-product-transaction.md) | Optional | - | getPrimaryLocation(): ?AccountVaultCauProductTransaction | setPrimaryLocation(?AccountVaultCauProductTransaction primaryLocation): void |
| `receivedEmails` | [`?(ReceivedEmail[])`](../../doc/models/received-email.md) | Optional | Received Email Information on `expand` | getReceivedEmails(): ?array | setReceivedEmails(?array receivedEmails): void |
| `contact` | [`?Contact3`](../../doc/models/contact-3.md) | Optional | - | getContact(): ?Contact3 | setContact(?Contact3 contact): void |
| `isDeletable` | `?bool` | Optional | Is Deletable Information on `expand` | getIsDeletable(): ?bool | setIsDeletable(?bool isDeletable): void |
| `activeNotificationAlerts` | [`?(ActiveNotificationAlert[])`](../../doc/models/active-notification-alert.md) | Optional | Active Notification Alert Information on `expand` | getActiveNotificationAlerts(): ?array | setActiveNotificationAlerts(?array activeNotificationAlerts): void |
| `locationUsers` | [`?(LocationUser[])`](../../doc/models/location-user.md) | Optional | Location User Information on `expand` | getLocationUsers(): ?array | setLocationUsers(?array locationUsers): void |
| `authRoles` | [`?(AuthRole[])`](../../doc/models/auth-role.md) | Optional | Auth Role Information on `expand` | getAuthRoles(): ?array | setAuthRoles(?array authRoles): void |
| `changelogs` | [`?(Changelog[])`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | getChangelogs(): ?array | setChangelogs(?array changelogs): void |
| `resources` | [`?Resources1`](../../doc/models/resources-1.md) | Optional | - | getResources(): ?Resources1 | setResources(?Resources1 resources): void |
| `domain` | [`?Domain1`](../../doc/models/domain-1.md) | Optional | - | getDomain(): ?Domain1 | setDomain(?Domain1 domain): void |
| `createdUser` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getCreatedUser(): ?User9 | setCreatedUser(?User9 createdUser): void |
| `locationMarketplaces` | [`?(Locationmarketplace[])`](../../doc/models/locationmarketplace.md) | Optional | Locationmarketplaces Information on `expand` | getLocationMarketplaces(): ?array | setLocationMarketplaces(?array locationMarketplaces): void |
| `emailBlacklist` | [`?EmailBlacklist1`](../../doc/models/email-blacklist-1.md) | Optional | - | getEmailBlacklist(): ?EmailBlacklist1 | setEmailBlacklist(?EmailBlacklist1 emailBlacklist): void |
| `helppage` | [`?Helppage`](../../doc/models/helppage.md) | Optional | - | getHelppage(): ?Helppage | setHelppage(?Helppage helppage): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "account_number": "5454545454545454",
  "branding_domain_url": "{branding_domain_url}",
  "cell_phone": "3339998822",
  "company_name": "Fortis Payment Systems, LLC",
  "contact_id": "Sample contact ID",
  "date_of_birth": "2021-12-01",
  "domain_id": "11e95f8ec39de8fbdb0a4f1a",
  "email": "email@domain.com",
  "email_trx_receipt": true,
  "home_phone": "3339998822",
  "first_name": "John",
  "last_name": "Smith",
  "locale": "en-US",
  "office_phone": "3339998822",
  "office_ext_phone": "5",
  "primary_location_id": "11e95f8ec39de8fbdb0a4f1a",
  "terms_condition_code": "20220308",
  "tz": "America/New_York",
  "username": "{user_name}",
  "user_api_key": "234bas8dfn8238f923w2",
  "zip": "48375",
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "api_only": false,
  "is_invitation": false,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "status": true,
  "login_attempts": 0,
  "last_login_ts": 1422040992,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "terms_accepted_ts": 1422040992,
  "terms_agree_ip": "192.168.0.10",
  "current_login": 1422040992,
  "log_api_response_body_ts": 1422040992,
  "isDeletable": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

