biocore
=======

[![NPM Package](https://img.shields.io/npm/v/biocore.svg?style=flat-square)](https://www.npmjs.org/package/biocore)
[![Build Status](https://travis-ci.org/biocoin/biocore.svg?branch=master)](https://travis-ci.org/biocoin/biocore)
[![Coverage Status](https://img.shields.io/coveralls/bitpay/bitcore.svg)](https://coveralls.io/r/bitpay/bitcore)

Infrastructure to build Biocoinand blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the biocore Library please see: https://github.com/biocoin/biocore-lib

## Getting Started

Before you begin you'll need to have Node.js v4 or v0.12 installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g biocore
```

Spin up a full node and join the network:

```bash
npm install -g biocore
biocore
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.biocore`.

Create a transaction:
```js
var biocore = require('biocore');
var transaction = new biocore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node](https://github.com/biocoin/biocore-node) - A full node with extended capabilities using BiocoinCore
- [Insight Via API](https://github.com/biocoin/insight-api) - A blockchain explorer HTTP API
- [Insight Via UI](https://github.com/biocoin/insight) - A blockchain explorer web user interface
- [Wallet Service](https://github.com/bitpay/bitcore-wallet-service) - A multisig HD service for wallets
- [Wallet Client](https://github.com/bitpay/bitcore-wallet-client) - A client for the wallet service
- [CLI Wallet](https://github.com/bitpay/bitcore-wallet) - A command-line based wallet client
- [Angular Wallet Client](https://github.com/bitpay/angular-bitcore-wallet-client) - An Angular based wallet client
- [Copay](https://github.com/bitpay/copay) - An easy-to-use, multiplatform, multisignature, secure biocoin wallet

## Libraries

- [Lib](https://github.com/biocoin/biocore-lib) - All of the core Biocoinprimatives including transactions, private key management and others
- [Payment Protocol](https://github.com/bitpay/bitcore-payment-protocol) - A protocol for communication between a merchant and customer
- [P2P](https://github.com/biocoin/biocore-p2p) - The peer-to-peer networking protocol
- [Mnemonic](https://github.com/bitpay/bitcore-mnemonic) - Implements mnemonic code for generating deterministic keys
- [Channel](https://github.com/bitpay/bitcore-channel) - Micropayment channels for rapidly adjusting biocoin transactions
- [Message](https://github.com/biocoin/biocore-message) - Biocoinmessage verification and signing
- [ECIES](https://github.com/bitpay/bitcore-ecies) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.


## Security

Please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/biocoin/biocore/blob/master/CONTRIBUTING.md) file.

This will generate files named `biocore.js` and `biocore.min.js`.

You can also use our pre-generated files, provided for each release along with a PGP signature by one of the project's maintainers. To get them, checkout a release commit (for example, https://github.com/bitpay/bitcore/commit/e33b6e3ba6a1e5830a079e02d949fce69ea33546 for v0.12.6).

To verify signatures, use the following PGP keys:
- @braydonf: https://pgp.mit.edu/pks/lookup?op=get&search=0x9BBF07CAC07A276D `D909 EFE6 70B5 F6CC 89A3 607A 9BBF 07CA C07A 276D`
- @gabegattis: https://pgp.mit.edu/pks/lookup?op=get&search=0x441430987182732C `F3EA 8E28 29B4 EC93 88CB  B0AA 4414 3098 7182 732C`
- @kleetus: https://pgp.mit.edu/pks/lookup?op=get&search=0x33195D27EF6BDB7F `F8B0 891C C459 C197 65C2 5043 3319 5D27 EF6B DB7F`
- @matiu: https://pgp.mit.edu/pks/lookup?op=get&search=0x9EDE6DE4DE531FAC `25CE ED88 A1B1 0CD1 12CD  4121 9EDE 6DE4 DE53 1FAC`

## License

Code released under [the MIT license](https://github.com/biocoin/biocore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2017 The biocoin Core Developer
