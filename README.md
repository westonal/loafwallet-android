![ƀ](/images/icon.png) loafwallet for Android
----------------------------------

[![download](images/icon-google-play.png)](https://play.google.com/store/apps/details?id=com.loafwallet)

## Litecoin done right

This is a Litecoin fork of the [breadwallet Android port](https://github.com/breadwallet/breadwallet-android) of the [breadwallet iOS app](https://github.com/breadwallet/breadwallet/).

## A completely standalone Litecoin wallet

Unlike many other Litecoin wallets, loafwallet is a real standalone Litecoin client. There is no server to get hacked
 or go down, so you can always access your money. Using [SPV](https://en.bitcoin
 .it/wiki/Thin_Client_Security#Header-Only_Clients) mode, loafwallet connects directly to the Litecoin network with
 the fast performance you need on a mobile device.

## The next step in wallet security

loafwallet is designed to protect you from malware, browser security holes,
*even physical theft*. With AES hardware encryption, app sandboxing, and verified boot, loafwallet represents a significant security advance over
web and desktop wallets.

## Beautiful simplicity

Simplicity is loafwallet's core design principle. A simple backup phrase is all you need to restore your wallet on
another device if yours is ever lost or broken. Because loafwallet is [deterministic](https://github
.com/bitcoin/bips/blob/master/bip-0032.mediawiki), your balance and transaction history can be recovered from just your backup phrase.

## Features

- ["simplified payment verification"](https://github.com/bitcoin/bips/blob/master/bip-0037.mediawiki) for fast mobile performance
- no server to get hacked or go down
- single backup phrase that works forever
- private keys never leave your device
- import [password protected](https://github.com/bitcoin/bips/blob/master/bip-0038.mediawiki) paper wallets
- ["payment protocol"](https://github.com/bitcoin/bips/blob/master/bip-0070.mediawiki) payee identity certification

## How to setup the development environment

1. Download and install Java 7 or up
2. Download and Install the latest Android studio
3. Download and install the latest NDK **v15** https://developer.android.com/ndk/downloads/index.html or download it in android studio by "choosing the NDK" and press "download". Note that v16 removes CPP support so **cannot be used**.
4. Go to https://github.com/litecoin-foundation/loafwallet-android and clone the project
5. Open the project with Android Studio and let the project sync
6. Go to SDK Manager and download all the SDK Platforms and SDK Tools
7. Initialize the submodules - `git submodule init`
8. Update the submodules - `git submodule update`
9. Build -> Rebuild Project or from command line `./gradlew assembleLoaf`
