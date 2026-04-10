
# Address Match

Indicates whether the Cardholder Shipping Address and Cardholder Billing Address are the same.
If the field is not set and the shipping and billing addresses are the same, the 3DS Server will set the value to Y. Otherwise, the value will not be changed.

> Y - Shipping Address matches Billing Address
> 
> N - Shipping Address does not match Billing Address

*This model accepts additional fields of type array.*

## Enumeration

`AddressMatch`

## Fields

| Name |
|  --- |
| `Y` |
| `N` |

## Example

```
N
```

