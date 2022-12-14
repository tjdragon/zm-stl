# zm-stl

Code to demonstrate atomic swap settlement for ERC20s

- [Gen20Token](https://github.com/tjdragon/zm-stl/blob/main/Gen20Token.sol) is a generic ERC20 implementation
- [ZETH](https://github.com/tjdragon/zm-stl/blob/main/ZETH.sol) is a wrapped ETH implementation with no re-entrancy issues. See more [here](https://halborn.com/what-is-a-re-entrancy-attack/)
- [IntercessorERC20V1](https://github.com/tjdragon/zm-stl/blob/main/IntercessorERC20V1.sol) is the smart contract that does the swap for ERC20s
- [IntercessorNativeV1](https://github.com/tjdragon/zm-stl/blob/main/IntercessorNativeV1.sol) is an investigation for handling native ETH. I do not recommend this approach and [ZETH](https://github.com/tjdragon/zm-stl/blob/main/ZETH.sol) should be used instead
- [IntercessorTestSeriesERC](https://github.com/tjdragon/zm-stl/blob/main/IntercessorTestSeriesERC.js) and [IntercessorTestSeriesNative](https://github.com/tjdragon/zm-stl/blob/main/IntercessorTestSeriesNative.js) are the test cases.


"An atomic swap is an exchange of cryptocurrencies from separate or identical blockchains. The swap is conducted between two entities without a third party's involvement. The idea is to remove centralized intermediaries like regulated exchanges and give token owners total control."

"The term atomic derives from the term "atomic state" in which a state has no substates; it either happens or it doesn't—there is no other alternative."

"Most atomic swap-enabled wallets and blockchains use smart contracts. Smart contracts are programs within blockchains that execute when certain conditions are met. In this case, the conditions are that each party agrees to the transaction before a timer runs out. Using a smart contract in the trade prevents either party from stealing a cryptocurrency from the other."

See more [here](https://www.investopedia.com/terms/a/atomic-swaps.asp) and about [HTLC here](https://corporatefinanceinstitute.com/resources/cryptocurrency/hashed-timelock-contract-htlc/)
