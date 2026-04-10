
# Three Ds Requestor

Contains information for the 3DS Requestor.

*This model accepts additional fields of type array.*

## Structure

`ThreeDsRequestor`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `threeDsRequestorAuthenticationInd` | [`string(ThreeDsRequestorAuthenticationInd)`](../../doc/models/three-ds-requestor-authentication-ind.md) | Required | - | getThreeDsRequestorAuthenticationInd(): string | setThreeDsRequestorAuthenticationInd(string threeDsRequestorAuthenticationInd): void |
| `threeDsRequestorAuthenticationInfo` | [`?(ThreeDsRequestorAuthenticationInfo[])`](../../doc/models/three-ds-requestor-authentication-info.md) | Optional | Information about how the 3DS Requestor authenticated the cardholder before or during the transaction. | getThreeDsRequestorAuthenticationInfo(): ?array | setThreeDsRequestorAuthenticationInfo(?array threeDsRequestorAuthenticationInfo): void |
| `threeDsRequestorChallengeInd` | [`?(string(ThreeDsRequestorChallengeInd)[])`](../../doc/models/three-ds-requestor-challenge-ind.md) | Optional | Indicates whether a challenge is requested for this transaction. For example: For 01-PA, a 3DS Requestor may have concerns about the transaction, and request a challenge. For 02-NPA, a challenge may be necessary when adding a new card to a wallet.<br><br>Values "05" through "09" are accepted as well if 3DS Server initiates authentication with EMV 3DS 2.2.0 version or greater (required protocol version can be set in the preferred_protocol_version field).<br><br>If the element is not provided, the expected action is that the ACS would interpret as 01 (No preference).<br><br>In versions prior to 2.3.1 only a single element is supported.  Starting from EMVCo version 2.3.1, this array can now support 1-2 elements.<br>When providing two preferences, you must ensure that they are in preference order and are not conflicting. For example, 02 = No challenge requested and 04 = Challenge requested (Mandate).<br><br>> 01 - No preference<br>> <br>> 02 - No challenge requested<br>> <br>> 03 - Challenge requested: 3DS Requestor Preference<br>> <br>> 04 - Challenge requested: Mandate<br>> <br>> 05 - No challenge requested (transactional risk analysis is already performed) (EMV 3DS 2.2.0 version or greater)<br>> <br>> 06 - No challenge requested (Data share only) (EMV 3DS 2.2.0 version or greater)<br>> <br>> 07 - No challenge requested (strong consumer authentication is already performed) (EMV 3DS 2.2.0 version or greater)<br>> <br>> 08 - No challenge requested (utilise whitelist exemption if no challenge required) (EMV 3DS 2.2.0 version or greater)<br>> <br>> 09 - Challenge requested (whitelist prompt requested if challenge required) (EMV 3DS 2.2.0 version or greater)<br>> <br>> 80 through 99 - can be used for PS-specific values, regardless of protocol version<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `2` | getThreeDsRequestorChallengeInd(): ?array | setThreeDsRequestorChallengeInd(?array threeDsRequestorChallengeInd): void |
| `threeDsRequestorPriorAuthenticationInfo` | [`?(ThreeDsRequestorPriorAuthenticationInfo[])`](../../doc/models/three-ds-requestor-prior-authentication-info.md) | Optional | This object contains information about how the 3DS Requestor authenticated the cardholder as part of a previous 3DS transaction.<br><br>In versions prior to 2.3.1, this array is limited to a size of 1.  Starting from EMVCo version 2.3.1 this array size may be 1-3.<br><br>This field is optional, but recommended to include for versions prior to 2.3.1. From 2.3.1, it is required for 3RI in the case of Decoupled Authentication Fallback or for SPC.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `3` | getThreeDsRequestorPriorAuthenticationInfo(): ?array | setThreeDsRequestorPriorAuthenticationInfo(?array threeDsRequestorPriorAuthenticationInfo): void |
| `threeDsRequestorDecReqInd` | [`?string(ThreeDsRequestorDecReqInd)`](../../doc/models/three-ds-requestor-dec-req-ind.md) | Optional | - | getThreeDsRequestorDecReqInd(): ?string | setThreeDsRequestorDecReqInd(?string threeDsRequestorDecReqInd): void |
| `threeDsRequestorDecMaxTime` | `?int` | Optional | Indicates the maximum amount of time that the 3DS Requestor will wait for an ACS to provide the results of a Decoupled Authentication transaction (in minutes). Valid values are between 1 and 10080.<br><br>The field is optional and if value is not present, the expected action is for the ACS to interpret it as 10080 minutes (7 days).<br>Available for supporting EMV 3DS 2.2.0 and later versions.<br><br>Starting from EMV 3DS 2.3.1:<br>This field is required if three_ds_requestor_dec_req_ind = Y, F or B | getThreeDsRequestorDecMaxTime(): ?int | setThreeDsRequestorDecMaxTime(?int threeDsRequestorDecMaxTime): void |
| `threeDsRequestorSpcSupport` | [`?string(ThreeDsRequestorSpcSupport)`](../../doc/models/three-ds-requestor-spc-support.md) | Optional | - | getThreeDsRequestorSpcSupport(): ?string | setThreeDsRequestorSpcSupport(?string threeDsRequestorSpcSupport): void |
| `spcIncompInd` | `?string` | Optional | Reason that the SPC authentication was not completed.<br>This field is required if device_channel = 02 (BRW) and the 3DS Requestor attempts to invoke SPC API and there is an error. Available for supporting EMV 3DS 2.3.1 and later versions. | getSpcIncompInd(): ?string | setSpcIncompInd(?string spcIncompInd): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "three_ds_requestor_authentication_ind": "98",
  "three_ds_requestor_challenge_ind": [
    "03"
  ],
  "three_ds_requestor_authentication_info": [
    {
      "three_ds_req_auth_method": "98",
      "three_ds_req_auth_timestamp": "three_ds_req_auth_timestamp2",
      "three_ds_req_auth_data": "three_ds_req_auth_data2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "three_ds_requestor_prior_authentication_info": [
    {
      "three_ds_req_prior_ref": "three_ds_req_prior_ref6",
      "three_ds_req_prior_auth_method": "90",
      "three_ds_req_prior_auth_timestamp": "three_ds_req_prior_auth_timestamp6",
      "three_ds_req_prior_auth_data": "three_ds_req_prior_auth_data0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "three_ds_req_prior_ref": "three_ds_req_prior_ref6",
      "three_ds_req_prior_auth_method": "90",
      "three_ds_req_prior_auth_timestamp": "three_ds_req_prior_auth_timestamp6",
      "three_ds_req_prior_auth_data": "three_ds_req_prior_auth_data0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "three_ds_req_prior_ref": "three_ds_req_prior_ref6",
      "three_ds_req_prior_auth_method": "90",
      "three_ds_req_prior_auth_timestamp": "three_ds_req_prior_auth_timestamp6",
      "three_ds_req_prior_auth_data": "three_ds_req_prior_auth_data0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "three_ds_requestor_dec_req_ind": "Y",
  "three_ds_requestor_dec_max_time": 236,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

