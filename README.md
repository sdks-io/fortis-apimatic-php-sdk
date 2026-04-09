
# Getting Started with Fortis API

## Install the Package

Run the following command to install the package and automatically add the dependency to your composer.json file:

```bash
composer require "fortis-apimatic/fortis-apimatic-sdk:1.0.0"
```

Or add it to the composer.json file manually as given below:

```json
"require": {
    "fortis-apimatic/fortis-apimatic-sdk": "1.0.0"
}
```

You can also view the package at:
https://packagist.org/packages/fortis-apimatic/fortis-apimatic-sdk#1.0.0

## Test the SDK

Unit tests in this SDK can be run using PHPUnit.

1. First install the dependencies using composer including the `require-dev` dependencies.
2. Run `vendor\bin\phpunit --verbose` from commandline to execute tests. If you have installed PHPUnit globally, run tests using `phpunit --verbose` instead.

You can change the PHPUnit test configuration in the `phpunit.xml` file.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/README.md#environments) | The API environment. <br> **Default: `Environment.SANDBOX`** |
| timeout | `int` | Timeout for API calls in seconds.<br>*Default*: `0` |
| enableRetries | `bool` | Whether to enable retries and backoff feature.<br>*Default*: `false` |
| numberOfRetries | `int` | The number of retries to make.<br>*Default*: `0` |
| retryInterval | `float` | The retry time interval between the endpoint calls.<br>*Default*: `1` |
| backOffFactor | `float` | Exponential backoff factor to increase interval between retries.<br>*Default*: `2` |
| maximumRetryWaitTime | `int` | The maximum wait time in seconds for overall retrying requests.<br>*Default*: `0` |
| retryOnTimeout | `bool` | Whether to retry on request timeout.<br>*Default*: `true` |
| httpStatusCodesToRetry | `array` | Http status codes to retry against.<br>*Default*: `408, 413, 429, 500, 502, 503, 504, 521, 522, 524` |
| httpMethodsToRetry | `array` | Http methods to retry against.<br>*Default*: `'GET', 'PUT'` |
| proxyConfiguration | [`ProxyConfigurationBuilder`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/proxy-configuration-builder.md) | Represents the proxy configurations for API calls |
| userIdCredentials | [`UserIdCredentials`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| userApiKeyCredentials | [`UserApiKeyCredentials`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature-1.md) | The Credentials Setter for Custom Header Signature |
| developerIdCredentials | [`DeveloperIdCredentials`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature-2.md) | The Credentials Setter for Custom Header Signature |
| accessTokenCredentials | [`AccessTokenCredentials`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature-3.md) | The Credentials Setter for Custom Header Signature |

The API client can be initialized as follows:

```php
use FortisAPILib\Environment;
use FortisAPILib\Authentication\UserIdCredentialsBuilder;
use FortisAPILib\Authentication\UserApiKeyCredentialsBuilder;
use FortisAPILib\Authentication\DeveloperIdCredentialsBuilder;
use FortisAPILib\Authentication\AccessTokenCredentialsBuilder;
use FortisAPILib\FortisAPIClientBuilder;

$client = FortisAPIClientBuilder::init()
    ->userIdCredentials(
        UserIdCredentialsBuilder::init(
            'user-id'
        )
    )
    ->userApiKeyCredentials(
        UserApiKeyCredentialsBuilder::init(
            'user-api-key'
        )
    )
    ->developerIdCredentials(
        DeveloperIdCredentialsBuilder::init(
            'developer-id'
        )
    )
    ->accessTokenCredentials(
        AccessTokenCredentialsBuilder::init(
            'access-token'
        )
    )
    ->environment(Environment::SANDBOX)
    ->build();
```

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| SANDBOX | **Default** |
| PRODUCTION | - |

## Authorization

This API uses the following authentication schemes.

* [`user-id (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature.md)
* [`user-api-key (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature-1.md)
* [`developer-id (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature-2.md)
* [`access-token (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/auth/custom-header-signature-3.md)

## List of APIs

* [Async Processing](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/async-processing.md)
* [Declined Recurring Transactions](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/declined-recurring-transactions.md)
* [Device Terms](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/device-terms.md)
* [Full Boarding](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/full-boarding.md)
* [3 DS Authentication](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/3-ds-authentication.md)
* [3 DS Transactions](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/3-ds-transactions.md)
* [Merchant Deposits](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/merchant-deposits.md)
* [On Boarding](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/on-boarding.md)
* [Payment Card Reader Token](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/payment-card-reader-token.md)
* [Quick Invoices](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/quick-invoices.md)
* [Transaction ACH Retries](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transaction-ach-retries.md)
* [Transactions-ACH](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transactions-ach.md)
* [Transactions-Cash](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transactions-cash.md)
* [Transactions-Credit Card](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transactions-credit-card.md)
* [Transactions-EBT Card](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transactions-ebt-card.md)
* [Transactions-Read](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transactions-read.md)
* [Level 3 Data](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/level-3-data.md)
* [Transactions-Updates](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/transactions-updates.md)
* [User Verifications](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/user-verifications.md)
* [Apple Pay Validate Merchant](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/apple-pay-validate-merchant.md)
* [Merchant Details](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/merchant-details.md)
* [Batches](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/batches.md)
* [Contacts](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/contacts.md)
* [Elements](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/elements.md)
* [Locations](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/locations.md)
* [Paylinks](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/paylinks.md)
* [Recurring](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/recurring.md)
* [Signatures](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/signatures.md)
* [Tags](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/tags.md)
* [Terminals](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/terminals.md)
* [Tickets](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/tickets.md)
* [Tokens](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/tokens.md)
* [Users](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/users.md)
* [Webhooks](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/controllers/webhooks.md)

## SDK Infrastructure

### Configuration

* [ProxyConfigurationBuilder](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/proxy-configuration-builder.md)

### HTTP

* [HttpRequest](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/http-request.md)
* [HttpResponse](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/http-response.md)

### Utilities

* [ApiException](https://www.github.com/sdks-io/fortis-apimatic-php-sdk/tree/1.0.0/doc/api-exception.md)

