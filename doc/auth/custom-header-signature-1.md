
# Custom Header Signature



Documentation for accessing and setting credentials for user-api-key.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| user-api-key | `string` | User API Key | `userApiKey` | `getUserApiKey()` |



**Note:** Auth credentials can be set using `UserApiKeyCredentialsBuilder::init()` in `userApiKeyCredentials` method in the client builder and accessed through `getUserApiKeyCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```php
use FortisApiLib\Authentication\UserApiKeyCredentialsBuilder;
use FortisApiLib\FortisApiClientBuilder;

$client = FortisApiClientBuilder::init()
    ->userApiKeyCredentials(
        UserApiKeyCredentialsBuilder::init(
            'user-api-key'
        )
    )
    ->build();
```


