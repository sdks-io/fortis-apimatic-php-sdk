
# Three Ds Requestor Authentication Info

*This model accepts additional fields of type array.*

## Structure

`ThreeDsRequestorAuthenticationInfo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `threeDsReqAuthMethod` | [`?string(ThreeDsReqAuthMethod)`](../../doc/models/three-ds-req-auth-method.md) | Optional | - | getThreeDsReqAuthMethod(): ?string | setThreeDsReqAuthMethod(?string threeDsReqAuthMethod): void |
| `threeDsReqAuthTimestamp` | `?string` | Optional | Date and time converted into UTC of the cardholder authentication. Field is limited to 12 characters and accepted format is YYYYMMDDHHMM<br><br>**Constraints**: *Maximum Length*: `12` | getThreeDsReqAuthTimestamp(): ?string | setThreeDsReqAuthTimestamp(?string threeDsReqAuthTimestamp): void |
| `threeDsReqAuthData` | `?string` | Optional | Stringified array of objects that documents and supports a specific authentication process. In the current version of the specification, this data element is not defined in detail, however the intention is that for each 3DS Requestor Authentication Method, this field carry data that the ACS can use to verify the authentication process. For example, if the 3DS<br>Requestor Authentication Method is:<br>03 -> then this element can carry information about the provider of the federated ID and related information<br>06 -> then this element can carry the FIDO attestation data (incl. the signature)<br>07 -> then this element can carry FIDO Attestation data with the FIDO assurance data signed.<br>08 -> then this element can carry the SRC assurance data.<br>In versions prior to 2.3.1, this array is limited to a single object.<br>Starting from EMVCo version 2.3.1, the array may have 1-3 elements.<br><br>This field is optional, but recommended to include.<br><br>**Constraints**: *Maximum Length*: `20000` | getThreeDsReqAuthData(): ?string | setThreeDsReqAuthData(?string threeDsReqAuthData): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "three_ds_req_auth_timestamp": "202403291556",
  "three_ds_req_auth_method": "90",
  "three_ds_req_auth_data": "three_ds_req_auth_data8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

