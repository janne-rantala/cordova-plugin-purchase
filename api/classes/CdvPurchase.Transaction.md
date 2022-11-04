# Class: Transaction

[CdvPurchase](../modules/CdvPurchase.md).Transaction

## Hierarchy

- **`Transaction`**

  ↳ [`SKTransaction`](CdvPurchase.AppleAppStore.SKTransaction.md)

  ↳ [`Transaction`](CdvPurchase.GooglePlay.Transaction.md)

## Table of contents

### Constructors

- [constructor](CdvPurchase.Transaction.md#constructor)

### Properties

- [expirationDate](CdvPurchase.Transaction.md#expirationdate)
- [isAcknowledged](CdvPurchase.Transaction.md#isacknowledged)
- [isConsumed](CdvPurchase.Transaction.md#isconsumed)
- [isPending](CdvPurchase.Transaction.md#ispending)
- [lastRenewalDate](CdvPurchase.Transaction.md#lastrenewaldate)
- [platform](CdvPurchase.Transaction.md#platform)
- [products](CdvPurchase.Transaction.md#products)
- [purchaseDate](CdvPurchase.Transaction.md#purchasedate)
- [purchaseId](CdvPurchase.Transaction.md#purchaseid)
- [renewalIntent](CdvPurchase.Transaction.md#renewalintent)
- [renewalIntentChangeDate](CdvPurchase.Transaction.md#renewalintentchangedate)
- [state](CdvPurchase.Transaction.md#state)
- [transactionId](CdvPurchase.Transaction.md#transactionid)

## Constructors

### constructor

• **new Transaction**(`platform`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `platform` | [`Platform`](../enums/CdvPurchase.Platform.md) |

## Properties

### expirationDate

• `Optional` **expirationDate**: `Date`

Time when the subscription is set to expire following this transaction

___

### isAcknowledged

• `Optional` **isAcknowledged**: `boolean`

True when the transaction has been acknowledged to the platform.

___

### isConsumed

• `Optional` **isConsumed**: `boolean`

True when the transaction was consumed.

___

### isPending

• `Optional` **isPending**: `boolean`

True when the transaction is still pending payment.

___

### lastRenewalDate

• `Optional` **lastRenewalDate**: `Date`

Time a subscription was last renewed

___

### platform

• **platform**: [`Platform`](../enums/CdvPurchase.Platform.md)

Platform this transaction was created on

___

### products

• **products**: { `offerId?`: `string` ; `productId`: `string`  }[] = `[]`

Purchased products

___

### purchaseDate

• `Optional` **purchaseDate**: `Date`

Time the purchase was made.

For subscriptions this is equal to the date of the first transaction.
Note that it might be undefined for deleted transactions (google for instance don't provide any info in that case).

___

### purchaseId

• `Optional` **purchaseId**: `string`

Identifier for the purchase this transaction is a part of.

___

### renewalIntent

• `Optional` **renewalIntent**: [`RenewalIntent`](../enums/CdvPurchase.RenewalIntent.md)

Is the subscription set to renew.

___

### renewalIntentChangeDate

• `Optional` **renewalIntentChangeDate**: `Date`

Time when the renewal intent was changed

___

### state

• **state**: [`TransactionState`](../enums/CdvPurchase.TransactionState.md) = `TransactionState.UNKNOWN_STATE`

State this transaction is in

___

### transactionId

• **transactionId**: `string` = `''`

Transaction identifier.