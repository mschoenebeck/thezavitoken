# The ZAVI Token

This is a sample application for private transactions on EOSIO using the Groth16/BLS12-381 SNARK verifier of the ZEOS token contract. This contract is deployed to the [Kylin Testnet](https://kylin.bloks.io/account/thezavitoken) and is part of the new [ZEOS Demo application](https://zeos.one/demo).

See also:
- [ZEOS Sapling](https://github.com/mschoenebeck/zeos-sapling)
- [JS Wallet (zavi)](https://github.com/mschoenebeck/zeos-wallet/tree/zavi)

## Description
This is a sample application for private transactions on EOSIO using the Groth16/BLS12-381 SNARK verifier of the ZEOS token contract. The ZAVI token contract has no DAPP dependencies nor does it need any DAPP tokens staked in order to use the SNARK verifier. All DAPP resources are being paid for by the ZEOS token contract. In order to call the `verifyproof` action of the ZEOS token contract it makes use of [EOSIO action wrappers](https://developers.eos.io/manuals/eosio.cdt/v1.7/how-to-guides/how_to_create_and_use_action_wrappers). The only dependency is the [ZEOSIO](https://github.com/mschoenebeck/zeosio) header-only library.

This contract is built on [EOSIO](https://eos.io/).

## Getting Started

To setup the full workspace clone the dependency [ZEOSIO](https://github.com/mschoenebeck/zeosio) as well:

```
mkdir zeos
cd zeos
git clone https://github.com/mschoenebeck/zeosio.git
```

Clone this repository:

```
git clone https://github.com/mschoenebeck/thezavitoken.git
cd thezavitoken
```

Build the contract:

```
cdt-cpp thezavitoken.cpp
```

### Dependencies

- [EOSIO Contract Development Toolkit (CDT)](https://github.com/EOSIO/eosio.cdt/releases)

## Help
If you need help join us on [Telegram](https://t.me/ZeosOnEos).

## Authors

Matthias Schönebeck

## License

It's open source. Do with it whatever you want.

## Acknowledgments

Big thanks to the Electric Coin Company for developing, documenting and maintaining this awesome open source codebase for zk-SNARKs!

* [Zcash Protocol Specification](https://zips.z.cash/protocol/protocol.pdf)
