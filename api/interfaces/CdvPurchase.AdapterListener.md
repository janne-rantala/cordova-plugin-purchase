# Interface: AdapterListener

[CdvPurchase](../modules/CdvPurchase.md).AdapterListener

## Table of contents

### Methods

- [productsUpdated](CdvPurchase.AdapterListener.md#productsupdated)
- [receiptsUpdated](CdvPurchase.AdapterListener.md#receiptsupdated)

## Methods

### productsUpdated

▸ **productsUpdated**(`platform`, `products`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `platform` | [`Platform`](../enums/CdvPurchase.Platform.md) |
| `products` | [`Product`](../classes/CdvPurchase.Product.md)[] |

#### Returns

`void`

___

### receiptsUpdated

▸ **receiptsUpdated**(`platform`, `receipts`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `platform` | [`Platform`](../enums/CdvPurchase.Platform.md) |
| `receipts` | [`Receipt`](../classes/CdvPurchase.Receipt.md)[] |

#### Returns

`void`