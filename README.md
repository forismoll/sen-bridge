# SEN Bridge

SEN is the currency of [Zen](https://myzen.today), a wallet that lives inside Telegram for payments, tips, games and communities. SEN was issued on TON with a fixed supply of 1,000,000.

SEN Bridge moves SEN between TON and BNB Smart Chain at a one to one rate.

- Bridge: https://myzen.today/bridge/
- Website: https://myzen.today
- X: https://x.com/MyZenWallet
- Telegram: https://t.me/zenwallet
- App in Telegram: https://t.me/SendZenBot

## How it works

- **TON to BNB Smart Chain.** SEN sent to the bridge is locked in the lockbox contract on TON, and the same amount of SEN is minted to the recipient on BNB Smart Chain.
- **BNB Smart Chain to TON.** SEN is burned on BNB Smart Chain, and the same amount is released from the lockbox on TON.
- Every transfer is approved by two of the bridge's three signers.
- SEN on BNB Smart Chain is minted only against SEN locked on TON, so the total supply across all networks stays at 1,000,000.

## Contracts

| Network | Contract | Address |
| --- | --- | --- |
| BNB Smart Chain (chain id 56) | SEN token (BEP-20, 9 decimals) | [`0xF9cA49b9DCAD63270553899494b9dc9E11687B02`](https://bscscan.com/token/0xF9cA49b9DCAD63270553899494b9dc9E11687B02) |
| BNB Smart Chain (chain id 56) | SenBridge (proxy) | [`0xf200a73aC8227eb7E23f591E2C178Ac0177753D7`](https://bscscan.com/address/0xf200a73aC8227eb7E23f591E2C178Ac0177753D7) |
| BNB Smart Chain (chain id 56) | SenBridge implementation | [`0xE9977B52c75660A52dC530E640FfbD7aAF48617e`](https://bscscan.com/address/0xE9977B52c75660A52dC530E640FfbD7aAF48617e) |
| TON | SEN jetton | [`EQA7MUqI2jT7y9_SiVJu3IMFmsMme0zLojFxLET3CzOqXzaA`](https://tonviewer.com/EQA7MUqI2jT7y9_SiVJu3IMFmsMme0zLojFxLET3CzOqXzaA) |
| TON | Bridge lockbox | [`EQBLJRWyoREYzgvfbFEhyU4q_6DAmoqHaFG4omn-4OkLDKOT`](https://tonviewer.com/EQBLJRWyoREYzgvfbFEhyU4q_6DAmoqHaFG4omn-4OkLDKOT) |
| Solana | SEN (via Wormhole, 8 decimals) | [`7ow8FhpdVjF6y9kXi6wXZUtPrVn8WzdY4CW7MSH63Xrh`](https://solscan.io/token/7ow8FhpdVjF6y9kXi6wXZUtPrVn8WzdY4CW7MSH63Xrh) |

The BNB Smart Chain contracts are verified on [Sourcify](https://sourcify.dev/#/lookup/0xF9cA49b9DCAD63270553899494b9dc9E11687B02).

Machine-readable addresses: [`deployments/bsc-mainnet.json`](deployments/bsc-mainnet.json).

## Markets

- BNB Smart Chain: [PancakeSwap v3 SEN/WBNB](https://pancakeswap.finance/info/v3/bsc/pairs/0x164eB601477968f478647CB033D4c9e9985e1fBD)
- TON: [STON.fi SEN/TON](https://app.ston.fi/pools/EQC5nAIZ8ymDEwITWbdEB8P4aLMAZugbnI9i_YZg7opOA7dk)
- Solana: [Meteora SEN/SOL](https://app.meteora.ag/dlmm/9BF7rqhaohQnufuTUS75Kk86LwNTMUSK1AtoHafvL2Ae)

## Contact

info@myzen.today
