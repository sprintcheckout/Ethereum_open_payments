
# Ethereum Open Payments Specification

![](https://i.imgur.com/uKSXryT.png)
### Scenario
Customer Bob pays 100USDC to Alice Flowers

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

### Appendix: ZK and Optmistic EVM rollups

- The Ethereum scalability approach for achieving security, speed, and cost-effective transaction gas fees is through ZK and Optmistic EVM compatible rollups.

### Appendix: Token allowance

- There needs to be a way to combine token allowance and transferFrom in order to save on transaction gas costs.

### Appendix: Chain agnostic

- Tokens hold in Ethereum should be transferrable in batch via 

---

## Specification
*work in progress*
### Wallet

### Payment dapps

### Bundler

### Paymaster

## Rational
Crypto payments are not widely accepted by merchants nowadays.
This specification aims to establish a standard that can be adopted by wallets, payment processing dapps (Web3 payment dapps), bundlers, and paymasters to provide a consistent payment experience that is easily recognizable by the general public.
We believe that combining a user-friendly experience with the scalability of zkEVMs and the security of Ethereum will web3 payments use case competitive with traditional payments.

## Goals
- Create a non-profit organization, for example named "Ethereum for Payments (E4P)", that any interested company can join.
- Establish branding and awareness among the general public, so that they can recognize and relate to the best-in-class payment experience.
- Develop a standard that web3 payment-related companies can follow.

## Get involved

#### Who should get involved
Any individual interested in Web3 payments, especially those with skills to contribute technically or in other areas such as content generation, community management, marketing, and branding, are welcome to participate. 

Additionally, any organization working on a component of ERC4337 (such as wallets, bundlers, and paymasters) or building services related to Web3 payments (such as wallets and payment processing) is encouraged to join.


#### How to contribute
- Contribute to this spec. Pull request to the repo available here https://github.com/sprintcheckout/Ethereum_for_payments/
- Join the Telegram group https://web.telegram.org/z/#-1785678853
- Join the list of official founding members, ask on the telegram group
- Create PR campaigns

#### Why to get involved
The development of zkEVMs and ERC4337 has created a new opportunity for decentralized payments that are scalable, fast, and secure. By working together as a group, we can strengthen each part of the ecosystem and onboard more effectively merchants and consumers to this new frontier of payments.


### Assets



![](https://i.imgur.com/cggSoY5.png =200x )

Easy to recognise Ethereum For Payments Org logo. It shall be displayed on ecommerce checkouts and wallets.

