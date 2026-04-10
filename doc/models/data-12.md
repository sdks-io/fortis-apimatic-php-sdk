
# Data 12

*This model accepts additional fields of type array.*

## Structure

`Data12`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `threeDsServerTransId` | `?string` | Optional | Universally unique transaction identifier assigned by the 3DS Server to identify a single transaction. It has the same value as the corresponding received authentication request. This value has 36 characters in a format defined in IETF RFC 4122.<br><br>**Constraints**: *Maximum Length*: `36` | getThreeDsServerTransId(): ?string | setThreeDsServerTransId(?string threeDsServerTransId): void |
| `acsUrl` | `?string` | Optional | Fully qualified URL of the ACS in case the authentication response message indicates that further Cardholder interaction is required to complete the authentication.<br><br>This field is only present in Browser flow. | getAcsUrl(): ?string | setAcsUrl(?string acsUrl): void |
| `transactionStatus` | [`?string(TransactionStatus)`](../../doc/models/transaction-status.md) | Optional | - | getTransactionStatus(): ?string | setTransactionStatus(?string transactionStatus): void |
| `authenticationValue` | `?string` | Optional | Payment System-specific value provided as part of the ACS registration for each supported DS. Authentication Value may be used to provide proof of authentication. | getAuthenticationValue(): ?string | setAuthenticationValue(?string authenticationValue): void |
| `eci` | `?string` | Optional | Payment System-specific value provided by the ACS to indicate the results of the attempt to authenticate the Cardholder. | getEci(): ?string | setEci(?string eci): void |
| `dsTransId` | `?string` | Optional | Universally unique transaction identifier assigned by the DS to identify a single transaction. | getDsTransId(): ?string | setDsTransId(?string dsTransId): void |
| `acsTransId` | `?string` | Optional | Universally unique transaction identifier assigned by the ACS to identify a single transaction. | getAcsTransId(): ?string | setAcsTransId(?string acsTransId): void |
| `messageVersion` | `?string` | Optional | Protocol version identifier This shall be the Protocol Version Number of the specification utilised by the system creating this message.<br>The Message Version Number is set by the 3DS Server which originates the protocol with the AReq message. The Message Version Number does not change during a 3DS transaction. | getMessageVersion(): ?string | setMessageVersion(?string messageVersion): void |
| `acsChallengeMandated` | [`?string(AcsChallengeMandated)`](../../doc/models/acs-challenge-mandated.md) | Optional | - | getAcsChallengeMandated(): ?string | setAcsChallengeMandated(?string acsChallengeMandated): void |
| `purchaseDate` | `?string` | Optional | Date and time of the purchase, converted into UTC. The field is limited to 14 characters, formatted as YYYYMMDDHHMMSS.<br><br>**Constraints**: *Maximum Length*: `14` | getPurchaseDate(): ?string | setPurchaseDate(?string purchaseDate): void |
| `base64EncodedChallengeRequest` | `?string` | Optional | Base64-encoded Challenge Request object in case the authentication response message indicates that further Cardholder interaction is required to complete the authentication. | getBase64EncodedChallengeRequest(): ?string | setBase64EncodedChallengeRequest(?string base64EncodedChallengeRequest): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "three_ds_server_trans_id": "ea0c9973-4cd0-4f9f-83b3-609bf22c69e7",
  "acs_url": "https://api.sandbox.fortis.tech/v1/acs/challenge",
  "ds_trans_id": "278c7508-cac6-4233-902d-b90f31f741c6",
  "acs_trans_id": "d7c1ee99-9478-44a6-b1f2-391e29c6b340",
  "message_version": "2.2.0",
  "purchase_date": "20240509111532",
  "base64_encoded_challenge_request": "eyJtZXNzYWdlVHlwZSI6IkNSZXEiLCJ0aHJlZURTU2VydmVyVHJhbnNJRCI6ImVhMGM5OTczLTRjZDAtNGY5Zi04M2IzLTYwOWJmMjJjNjllNyIsImFjc1RyYW5zSUQiOiIwNWViNTE2OS02ZTFkLTQ5NTMtYWQ3NC1hZWU5YmQ4ZTc1YmIiLCJjaGFsbGVuZ2VXaW5kb3dTaXplIjoiMDEiLCJtZXNzYWdlVmVyc2lvbiI6IjIuMi4wIn0=",
  "transaction_status": "R",
  "authentication_value": "authentication_value0",
  "eci": "eci8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

