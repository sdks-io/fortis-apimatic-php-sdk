# 3 DS Transactions

```php
$m3DsTransactionsController = $client->getM3DsTransactionsController();
```

## Class Name

`M3DsTransactionsController`


# 3 DS Transactions Request

For getting results of successful 3DS authentication attempts

```php
function m3DsTransactionsRequest(string $threeDsServerTransId, string $productTransactionId): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `threeDsServerTransId` | `string` | Template, Required | Universally unique transaction identifier assigned by the 3DS Server to identify a single transaction. |
| `productTransactionId` | `string` | Query, Required | Product Transaction ID associated with this 3DS request<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`ResponseThreeDsTransaction`](../../doc/models/response-three-ds-transaction.md).

## Example Usage

```php
$threeDsServerTransId = '516ef0bf-e510-4895-b0a8-c889f2eaf471';

$productTransactionId = '11e95f8ec39de8fbdb0a4f1a';

$m3DsTransactionsController = $client->getM3DsTransactionsController();
$apiResponse = $m3DsTransactionsController->m3DsTransactionsRequest(
    $threeDsServerTransId,
    $productTransactionId
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'ResponseThreeDsTransaction:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```

## Example Response *(as JSON)*

```json
{
  "type": "ThreeDSTransaction",
  "data": {
    "three_ds_server_trans_id": "516ef0bf-e510-4895-b0a8-c889f2eaf471",
    "transaction_status": "Y",
    "ds_trans_id": "f25084f0-5b16-4c0a-ae5d-b24808a95e4b",
    "acs_trans_id": "d7c1ee99-9478-44a6-b1f2-391e29c6b340",
    "message_version": "2.2.0",
    "authentication_value": "MTIzNDU2Nzg5MDA5ODc2NTQzMjE=",
    "eci": "05"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |

