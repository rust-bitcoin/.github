# Rust Bitcoin Community

A Series of projects to implement various Bitcoin protocols in Rust.

## TL;DR;

`rust-bitcoin` hosts the [`bitcoin`](https://crates.io/crates/bitcoin) crate that supports the
Bitcoin network protocol and associated primitives. It is designed for Rust programs built to work
with the Bitcoin network.

## Core Crates

The "core" crates developed and maintained collectively by the `rust-bitcoin` devs. There is a list
of official [maintainers](https://github.com/rust-bitcoin/rust-bitcoin/blob/master/CONTRIBUTING.md#repository-maintainers)
for the `bitcoin` crate, for other crates please see the git index to get an idea of who is who.

For these crates we hold ourselves to high standards relating to security, testing, release
schedule, API design, and coding style. Our current focus is on stabilizing these crates[^0].

Name | Crate | Repository
---|---|---
base58 | [base58ck](https://crates.io/crates/base58ck) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)
bitcoin | [bitcoin](https://crates.io/crates/bitcoin) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)
bitcoinconsensus | [bitcoinconsensus](https://crates.io/crates/bitcoinconsensus) | [rust-bitcoinconsensus](https://github.com/rust-bitcoin/rust-bitcoinconsensus)
bech32 | [bech32](https://crates.io/crates/bech32) | [rust-bech32](https://github.com/rust-bitcoin/rust-bech32)
chacha20_poly1305 | [chacha20-poly1305](https://crates.io/crates/chacha20-poly1305) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)
hashes | [bitcoin_hashes](https://crates.io/crates/bitcoin_hashes) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)
hex | [hex-conservative](https://crates.io/crates/hex-conservative) | [hex-conservative](https://github.com/rust-bitcoin/hex-conservative)
internals | [bitcoin-internals](https://crates.io/crates/bitcoin-internals) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)
io | [bitcoin-io](https://crates.io/crates/bitcoin-io) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)
ordered | [ordered](https://crates.io/crates/ordered) | [rust-ordered](https://github.com/rust-bitcoin/rust-ordered)
secp256k1 | [secp256k1](https://crates.io/crates/secp256k1) | [rust-secp256k1](https://github.com/rust-bitcoin/rust-secp256k1)
units | [bitcoin-units](https://crates.io/crates/bitcoin-units) | [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)

We aim to make usage of these crates secure, ergonomic, and intuitive. We try to enable users of
these crates to follow software engineering best practices e.g., semver compliance.

If we fall short of these stated aims, or can in anyway improve our support of Bitcoin free software
projects, please raise issues or contact maintainers directly. For security related issues please
see [SECURITY.md](https://github.com/rust-bitcoin/rust-bitcoin/blob/master/SECURITY.md).

If you write proprietary software and want better integration with these crates by all means raise
issues on the respective repository. We are interested in all users and your usecase may help us
improve the libraries, however all development is done in the open and will stay that way.

[^0]: Please note `internals` will explicitly never stabalize.

## Other Crates

Other crates/repositories hosted here and developed and maintained by the community.

These crates are developed and maintained by a subset of the `rust-bitcoin` devs or other members of
the community. We are fairly open about hosting any Bitcoin-related crates in this organization, provided
that they are actively maintained. Other requirements are:

- The repository contains Bitcoin-specific crates (implies Bitcoin-only and not general purpose crates).
- The repository has at least minimal CI.
- The author has made at least some effort to adhere to practices and standards maintained in the
  core crates (defined above).

These crates may not be reviewed or maintained by the primary `rust-bitcoin` maintainers. Keep this in
mind when choosing to use them as dependencies. And as with any dependencies, you should review new
versions rather than blindly upgrading.

Name | Crate | Repository
---|---|---
miniscript | [miniscript](https://crates.io/crates/miniscript) | [rust-miniscript](https://github.com/rust-bitcoin/rust-miniscript)
bitcoind | [bitcoind](https://crates.io/crates/bitcoind) | [bitcoind](https://github.com/rust-bitcoin/bitcoind)
bitcoincore-rpc | [bitcoincore-rpc](https://crates.io/crates/bitcoincore-rpc) | [rust-bitcoincore-rpc](https://github.com/rust-bitcoin/rust-bitcoincore-rpc)
bip39 | [bip39](https://crates.io/crates/bip39) | [rust-bip39](https://github.com/rust-bitcoin/rust-bip39)
bip47 | [bip47](https://crates.io/crates/bip47) | [rust-bip47](https://github.com/rust-bitcoin/rust-bip47)
bip322 | [bip322](https://crates.io/crates/bip322) | [bip322](https://github.com/rust-bitcoin/bip322)
murmel | [murmel](https://crates.io/crates/murmel) | [murmel](https://github.com/rust-bitcoin/murmel)
hammersbald | [hammersbald](https://crates.io/crates/hammersbald) | [hammersbald](https://github.com/rust-bitcoin/hammersbald)
bitcoin-bech32 | [bitcoin-bech32](https://crates.io/crates/bitcoin-bech32) | [rust-bech32-bitcoin](https://github.com/rust-bitcoin/rust-bech32-bitcoin)
corepc | [corepc](https://crates.io/crates/corepc-node) | [corepc](https://github.com/rust-bitcoin/corepc)
bitcoin-payment-instructions | [bitcoin-payment-instructions](https://crates.io/crates/bitcoin-payment-instructions) | [bitcoin-payment-instructions](https://github.com/rust-bitcoin/bitcoin-payment-instructions)

## Non-crate repositories

Repositories that are not crates (libraries).

Name | Repository | Description
---|---|---
maintainer-tools | [rust-bitcoin-maintainer-tools](https://github.com/rust-bitcoin/rust-bitcoin-maintainer-tools) | Scripts, test vectors, and other things used by or across multiple repositories in the `rust-bitcoin` ecosystem.
website | [rust-bitcoin.github.io](https://github.com/rust-bitcoin/rust-bitcoin.github.io) | Source for the organization website https://rust-bitcoin.org
workshop | [workshop](https://github.com/rust-bitcoin/) | Conference presentation material
.github | [.github](https://github.com/rust-bitcoin/) | Hosts this readme file

## Archived crates

These crates have either been moved to another location or are no longer actively maintained.

Repository | Crate or Description
---|---
rust-wallet | Unmaintained [bitcoin-wallet](https://crates.io/crates/bitcoin-wallet)
rust-bitcoin-chain | Unmaintained [bitcoin-chain](https://github.com/rust-bitcoin/rust-bitcoin-chain)
bitcoin_hashes | Moved to [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin/tree/master/hashes)
rust-lightning-invoice | Moved to [rust-lightning](https://github.com/lightningdevkit/rust-lightning/tree/main/lightning-invoice)
www.rust-bitcoin.org | Moved to [rust-bitcoin.github.io](https://github.com/rust-bitcoin/rust-bitcoin.github.io)
bitcoind-json-rpc-client | Unmaintained [bitcoind-json-rpc-client](https://crates.io/crates/bitcoind-json-rpc-client)
bitcoind-json-rpc-regtest | Unmaintained [bitcoind-json-rpc-regtest](https://crates.io/crates/bitcoind-json-rpc-regtest)
bitcoind-json-rpc-types | Unmaintained [bitcoind-json-rpc-types](https://crates.io/crates/bitcoind-json-rpc-types)

## TODO

- [constants](https://github.com/rust-bitcoin/constants): https://github.com/rust-bitcoin/constants/issues/9
- https://github.com/rust-bitcoin/rust-bech32-bitcoin/issues/39
