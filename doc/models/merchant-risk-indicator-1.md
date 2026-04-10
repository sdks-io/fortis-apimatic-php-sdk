
# Merchant Risk Indicator 1

*This model accepts additional fields of type array.*

## Structure

`MerchantRiskIndicator1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `shipIndicator` | [`?string(ShipIndicator)`](../../doc/models/ship-indicator.md) | Optional | - | getShipIndicator(): ?string | setShipIndicator(?string shipIndicator): void |
| `deliveryTimeframe` | [`?string(DeliveryTimeframe)`](../../doc/models/delivery-timeframe.md) | Optional | - | getDeliveryTimeframe(): ?string | setDeliveryTimeframe(?string deliveryTimeframe): void |
| `deliveryEmailAddress` | `?string` | Optional | For electronic delivery, the email address to which the merchandise was delivered. | getDeliveryEmailAddress(): ?string | setDeliveryEmailAddress(?string deliveryEmailAddress): void |
| `reorderItemsInd` | [`?string(ReorderItemsInd)`](../../doc/models/reorder-items-ind.md) | Optional | - | getReorderItemsInd(): ?string | setReorderItemsInd(?string reorderItemsInd): void |
| `preOrderPurchaseInd` | [`?string(PreOrderPurchaseInd)`](../../doc/models/pre-order-purchase-ind.md) | Optional | - | getPreOrderPurchaseInd(): ?string | setPreOrderPurchaseInd(?string preOrderPurchaseInd): void |
| `preOrderDate` | `?string` | Optional | For a pre-ordered purchase, the expected date that the merchandise will be available. Date format must be YYYYMMDD. | getPreOrderDate(): ?string | setPreOrderDate(?string preOrderDate): void |
| `giftCardAmount` | `?int` | Optional | For prepaid or gift card purchase, the purchase amount total of prepaid or gift card(s) in major units (for example, USD 123.45 is 123). | getGiftCardAmount(): ?int | setGiftCardAmount(?int giftCardAmount): void |
| `giftCardCurr` | `?string` | Optional | For prepaid or gift card purchase, the currency code of the card as defined in ISO 4217 except 955 - 964 and 999. | getGiftCardCurr(): ?string | setGiftCardCurr(?string giftCardCurr): void |
| `giftCardCount` | `?int` | Optional | For prepaid or gift card purchase, total count of individual prepaid or gift cards/codes purchased.<br><br>**Constraints**: `>= 0`, `<= 99` | getGiftCardCount(): ?int | setGiftCardCount(?int giftCardCount): void |
| `transChar` | [`?(string(TransChar)[])`](../../doc/models/trans-char.md) | Optional | Available starting in EMV 3DS 2.3.1.1.  Indicates to the ACS specific transactions identified by the Merchant.<br><br>> 01 - Cryptocurrency transaction<br>> <br>> 02 - NFT transaction<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `2` | getTransChar(): ?array | setTransChar(?array transChar): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "delivery_email_address": "fortis@example.com",
  "ship_indicator": "01",
  "delivery_timeframe": "01",
  "reorder_items_ind": "01",
  "pre_order_purchase_ind": "01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

