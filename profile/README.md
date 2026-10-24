# PISA

Payjoin with cross-input signature aggregation (CISA): a payjoin whose inputs,
from two wallets share one BIP 460 signature. A prototype on regtest only.

https://github.com/user-attachments/assets/5ee1d013-1b68-4482-844b-a450807f5873

| Part | Repository | Branch |
|------|------------|--------|
| Demo: two wallets, a PISA transfer, and the video | [pisa-demo](https://github.com/bitcoin-pisa/pisa-demo) | `main` |
| Async Payjoin (BIP 77) with full aggregation: protocol profile and prototype | [pisa](https://github.com/bitcoin-pisa/pisa) | `main` |
| Bitcoin Core with BIP 460, the code of [bitcoin#36122](https://github.com/bitcoin/bitcoin/pull/36122) | [bitcoin](https://github.com/bitcoin-pisa/bitcoin/tree/bip460) | `bip460` |
| Payjoin library that carries the CISA PSBT fields | [rust-payjoin](https://github.com/bitcoin-pisa/rust-payjoin/tree/cisa-psbt-carriage) | `cisa-psbt-carriage` |
| Explorer that shows aggregated signatures, the savings, and who is who in a payjoin | [mempool](https://github.com/bitcoin-pisa/mempool/tree/cisa-witness-v2) | `cisa-witness-v2` |

To run it, start with the [pisa-demo README](https://github.com/bitcoin-pisa/pisa-demo#run-it).

Specifications: [BIP 458](https://github.com/bitcoin/bips/pull/2205) half
aggregation, [BIP 459](https://github.com/bitcoin/bips/pull/2210) full
aggregation, [BIP 460](https://github.com/bitcoin/bips/pull/2212) CISA for
Taproot key path spends.
