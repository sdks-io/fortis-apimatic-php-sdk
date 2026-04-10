
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](../README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| timeout | `int` | Timeout for API calls in seconds.<br>*Default*: `0` |
| enableRetries | `bool` | Whether to enable retries and backoff feature.<br>*Default*: `false` |
| numberOfRetries | `int` | The number of retries to make.<br>*Default*: `0` |
| retryInterval | `float` | The retry time interval between the endpoint calls.<br>*Default*: `1` |
| backOffFactor | `float` | Exponential backoff factor to increase interval between retries.<br>*Default*: `2` |
| maximumRetryWaitTime | `int` | The maximum wait time in seconds for overall retrying requests.<br>*Default*: `0` |
| retryOnTimeout | `bool` | Whether to retry on request timeout.<br>*Default*: `true` |
| httpStatusCodesToRetry | `array` | Http status codes to retry against.<br>*Default*: `408, 413, 429, 500, 502, 503, 504, 521, 522, 524` |
| httpMethodsToRetry | `array` | Http methods to retry against.<br>*Default*: `'GET', 'PUT'` |
| loggingConfiguration | [`LoggingConfigurationBuilder`](../doc/logging-configuration-builder.md) | Represents the logging configurations for API calls |
| proxyConfiguration | [`ProxyConfigurationBuilder`](../doc/proxy-configuration-builder.md) | Represents the proxy configurations for API calls |
| userIdCredentials | [`UserIdCredentials`](auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| userApiKeyCredentials | [`UserApiKeyCredentials`](auth/custom-header-signature-1.md) | The Credentials Setter for Custom Header Signature |
| developerIdCredentials | [`DeveloperIdCredentials`](auth/custom-header-signature-2.md) | The Credentials Setter for Custom Header Signature |
| accessTokenCredentials | [`AccessTokenCredentials`](auth/custom-header-signature-3.md) | The Credentials Setter for Custom Header Signature |

The API client can be initialized as follows:

```php
use FortisApiLib\Logging\LoggingConfigurationBuilder;
use FortisApiLib\Logging\RequestLoggingConfigurationBuilder;
use FortisApiLib\Logging\ResponseLoggingConfigurationBuilder;
use Psr\Log\LogLevel;
use FortisApiLib\Environment;
use FortisApiLib\Authentication\UserIdCredentialsBuilder;
use FortisApiLib\Authentication\UserApiKeyCredentialsBuilder;
use FortisApiLib\Authentication\DeveloperIdCredentialsBuilder;
use FortisApiLib\Authentication\AccessTokenCredentialsBuilder;
use FortisApiLib\FortisApiClientBuilder;

$client = FortisApiClientBuilder::init()
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
    ->environment(Environment::PRODUCTION)
    ->loggingConfiguration(
        LoggingConfigurationBuilder::init()
            ->level(LogLevel::INFO)
            ->requestConfiguration(RequestLoggingConfigurationBuilder::init()->body(true))
            ->responseConfiguration(ResponseLoggingConfigurationBuilder::init()->headers(true))
    )
    ->build();
```

## Fortis API Client

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

## Controllers

| Name | Description |
|  --- | --- |
| getAsyncProcessingController() | Gets AsyncProcessingController |
| getBatchesController() | Gets BatchesController |
| getContactsController() | Gets ContactsController |
| getDeclinedRecurringTransactionsController() | Gets DeclinedRecurringTransactionsController |
| getDeviceTermsController() | Gets DeviceTermsController |
| getElementsController() | Gets ElementsController |
| getFullBoardingController() | Gets FullBoardingController |
| getLocationsController() | Gets LocationsController |
| getM3DsAuthenticationController() | Gets M3DsAuthenticationController |
| getM3DsTransactionsController() | Gets M3DsTransactionsController |
| getMerchantDepositsController() | Gets MerchantDepositsController |
| getOnBoardingController() | Gets OnBoardingController |
| getPaylinksController() | Gets PaylinksController |
| getPaymentCardReaderTokenController() | Gets PaymentCardReaderTokenController |
| getQuickInvoicesController() | Gets QuickInvoicesController |
| getRecurringController() | Gets RecurringController |
| getSignaturesController() | Gets SignaturesController |
| getTagsController() | Gets TagsController |
| getTerminalsController() | Gets TerminalsController |
| getTicketsController() | Gets TicketsController |
| getTokensController() | Gets TokensController |
| getTransactionAchRetriesController() | Gets TransactionAchRetriesController |
| getTransactionsAchController() | Gets TransactionsAchController |
| getTransactionsCashController() | Gets TransactionsCashController |
| getTransactionsCreditCardController() | Gets TransactionsCreditCardController |
| getTransactionsEbtCardController() | Gets TransactionsEbtCardController |
| getTransactionsReadController() | Gets TransactionsReadController |
| getLevel3DataController() | Gets Level3DataController |
| getTransactionsUpdatesController() | Gets TransactionsUpdatesController |
| getUserVerificationsController() | Gets UserVerificationsController |
| getUsersController() | Gets UsersController |
| getApplePayValidateMerchantController() | Gets ApplePayValidateMerchantController |
| getMerchantDetailsController() | Gets MerchantDetailsController |
| getWebhooksController() | Gets WebhooksController |

