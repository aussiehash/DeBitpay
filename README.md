# DeBitpay

> Does your Bitcoin wallet not support Bitpay payments? DeBitpay is a simple app which decodes Bitpay payment links into Bitcoin transaction requirements, so that you could make the payments with Bitcoin wallets not supporting Bitpay.

Open DeBitpay: [https://alexk111.github.io/DeBitpay/](https://alexk111.github.io/DeBitpay/) (hosted on GitHub via [https://github.com/alexk111/DeBitpay/tree/gh-pages](gh-pages) branch consisting of built /dist files)

## Story Behind the App

I make Bitcoin payments thru Bitpay from time to time. Everything went good until someday they started forcing payers to use their payment protocol and hiding native Bitcoin addresses on the invoice pages. If the wallet you use supports the protocol, then you don't have problems with that, but what about those who use wallets not supporting it? First there were a hackish way of getting output addresses by changing the invoice url to *invoice-noscript*. When that stopped working, someone found [another way](https://www.garyshood.com/bitpay/). After a while this one also stopped showing the transaction details. I couldn't tolerate this anymore and decided to make a long-lasting solution that gets the transaction requirements the same way the wallets supporting Bitpay do, and unveils the data so that Bitpay transactions could be made with any Bitcoin wallet.

## Security Note

Due to a missing header in responses from Bitpay servers I had to skip a hash verification of Bitpay data. More details on [DeBitpay (NodeJS edition) repo](https://github.com/alexk111/DeBitpay-nodejs).

## Installing on your system

1. [Download DeBitpay](https://github.com/alexk111/DeBitpay/archive/master.zip) from GitHub.
2. Unpack the downloaded zip and install dependencies:

```
npm install
```

## Build

```
npm run build
```

The command will build the app in /dist folder.

## Open

Go to /dist folder and open *index.html* with your browser.

## License

MIT © Alex Kaul


