
# ERC4337 For Payments Specification (E4P)

![](https://i.imgur.com/uKSXryT.png)
### Scenario
Customer Bob pays 100USDC to the Merchant Alice Flowers

### Events

**(1) The user pays for the purchase**

- To complete a purchase worth 100 USD, the user must send 100 USDC only, which should include the fees.

**(2) The merchant covers gas and service fees**

- When a purchase is made for 100USD, the merchant receives 99USDC and pays 1USDC for transaction gas and service fees.

**(3) The wallet provider is rewarded**

- The payment processor splits a portion of the service fee with the wallet provider.

 **(4)  The payment processor pays the gas in ETH**

- The paymaster will calculate the cost of the transaction in ETH and have the necessary funds available to complete it. The paymaster will then subtract the corresponding amount in USDC from the merchant.

**(5) The payment processor is rewarded**

- The paymaster transfers funds to the wallet provider and sets aside a budget that is equivalent to the amount of ETH spent on gas. The merchant's service fees are calculated as the remaining amount.

### Appendix: Subscriptions

- The payment processors should be able to obtain the user's authorization to carry out transactions for a fixed or varying amount on a monthly or specified basis.

### Appendix: zkEVMS

- The Ethereum scalability approach for achieving security, speed, and cost-effective transaction gas fees is through zkEVMs.

### Appendix: Token allowance

- There needs to be a way to combine token allowance and transferFrom in order to save on transaction gas costs.

---

## Specification

*The following ERC4337 elements must work together to meet the requirements listed above.*

### UserOperation 

### Sender

### EntryPoint

### Bundler 

### Aggregator

### Paymaster