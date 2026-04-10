# Payment Card Reader Token

```php
$paymentCardReaderTokenController = $client->getPaymentCardReaderTokenController();
```

## Class Name

`PaymentCardReaderTokenController`


# Payment Card Reader Token Request

For initializing iPhone card readers for Apple Tap to Pay transactions

```php
function paymentCardReaderTokenRequest(string $productTransactionId): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `productTransactionId` | `string` | Query, Required | Product Transaction ID to be used to initialize the card reader<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`ResponsePaymentCardReaderToken`](../../doc/models/response-payment-card-reader-token.md).

## Example Usage

```php
$productTransactionId = '11e95f8ec39de8fbdb0a4f1a';

$paymentCardReaderTokenController = $client->getPaymentCardReaderTokenController();
$apiResponse = $paymentCardReaderTokenController->paymentCardReaderTokenRequest($productTransactionId);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'ResponsePaymentCardReaderToken:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```

## Example Response *(as JSON)*

```json
{
  "type": "PaymentCardReaderToken",
  "data": {}
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401TokenException`](../../doc/models/response-401-token-exception.md) |

