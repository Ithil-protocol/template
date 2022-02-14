# Ithil

Ithil v1 core smart contracts.

## Main

Key infrastructural components.

- **Vault**: responsible for bookkeeping of loans, repayments and handling LP staking and unstaking issuing a yield-bearing token, the _Vault_ consists of several _subvaults_ each for each ERC20 token whitelisted and is independent from the others.

- **WrappedToken**: the yield-bearing token minted to the staker as a proof of deposit that can be withdrawn in exchange for the underlying asset deposited in the _Vault_.

## Strategies

Supported strategies.

- **BaseStrategy**: abstract parent contract for all strategies containing risk factors for the whitelisted tokens and the address of the _Vault_.

- **MarginTradingStrategy**: going short or long on any token pair using Kyber network

## Mocks

Useful for testing purposes, their name suggests the function.
