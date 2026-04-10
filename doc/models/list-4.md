
# List 4

*This model accepts additional fields of type array.*

## Structure

`List4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `locationId` | `?string` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `terminalId` | `?string` | Optional | Terminal ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getTerminalId(): ?string | setTerminalId(?string terminalId): void |
| `requireSignature` | `?bool` | Optional | Set to true or 1 to require a signature from the customer | getRequireSignature(): ?bool | setRequireSignature(?bool requireSignature): void |
| `deviceTermApiId` | `?string` | Optional | Can be used for associating record to external systems. Must be unique per location.<br><br>**Constraints**: *Maximum Length*: `64` | getDeviceTermApiId(): ?string | setDeviceTermApiId(?string deviceTermApiId): void |
| `termsConditions` | `?string` | Optional | This is the message that is displayed on the screen when prompting for a signature.<br><br>**Constraints**: *Maximum Length*: `4096` | getTermsConditions(): ?string | setTermsConditions(?string termsConditions): void |
| `id` | `?string` | Optional | Device term ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `reasonCodeId` | `?int` | Optional | Reason code ID | getReasonCodeId(): ?int | setReasonCodeId(?int reasonCodeId): void |
| `signature` | [`?Signature1`](../../doc/models/signature-1.md) | Optional | - | getSignature(): ?Signature1 | setSignature(?Signature1 signature): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `modifiedTs` | `?int` | Optional | Modified Time Stamp | getModifiedTs(): ?int | setModifiedTs(?int modifiedTs): void |
| `createdUserId` | `?string` | Optional | System generated id for user who created record<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCreatedUserId(): ?string | setCreatedUserId(?string createdUserId): void |
| `createdUser` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getCreatedUser(): ?User9 | setCreatedUser(?User9 createdUser): void |
| `location` | [`?Location18`](../../doc/models/location-18.md) | Optional | - | getLocation(): ?Location18 | setLocation(?Location18 location): void |
| `terminal` | [`?Terminal2`](../../doc/models/terminal-2.md) | Optional | - | getTerminal(): ?Terminal2 | setTerminal(?Terminal2 terminal): void |
| `changelogs` | [`?(Changelog[])`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | getChangelogs(): ?array | setChangelogs(?array changelogs): void |
| `reasonCode` | [`?ReasonCode1`](../../doc/models/reason-code-1.md) | Optional | - | getReasonCode(): ?ReasonCode1 | setReasonCode(?ReasonCode1 reasonCode): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "terminal_id": "11e95f8ec39de8fbdb0a4f1a",
  "require_signature": true,
  "device_term_api_id": "device_term134",
  "terms_conditions": "FUNgib0Vh0B9c0Wbttvr50vNtGLOkTdFL0eFmhN1RJpKhK14IENeDa8irp2dEk9thEcVHvVEyriQeZLs5NjNsCzqNj9JDA4RSJwK647IFtYjrNPN1nBb9bw6hoQ71oT5kpsiXGt8HcqBFVBVeDA7psIzKAyDveAw2o1hfjipkOtXrPgWun0rYwyyFuvqkT1egQYKfYDj",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "reason_code_id": 1000,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

