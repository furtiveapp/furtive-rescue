# Furtive Rescue

Take everything out of your Furtive account with nothing but your 12 words.

Furtive Rescue is a single page that runs entirely on your device. It reads the blockchain directly, makes the zero-knowledge proofs locally, and sends your full balance to any wallet you choose. It does not use Furtive's servers or website, so it keeps working even if they are unreachable.

## Use it

- **Online:** open the hosted copy of this repository's `index.html`.
- **Offline:** download `index.html` and open it in any modern browser. It contains everything it needs.

You will need your 12 words, a wallet address to receive your funds, and a small amount of ETH on Robinhood Chain for the network fee. The page tells you exactly how much and where to send it.

## Verify your copy

```
sha256  6ad67a00840adafb619b38e64d74c2ad3c4c6db0b59afc52f7cedc0413956efc  index.html
```

## How it works

Furtive keeps funds in a vault contract with no owner. Anyone can submit a withdrawal; only a valid proof made with your key decides what happens. This page derives your keys from your 12 words, finds your notes in the vault, proves each withdrawal on your device and submits it from your own drop-off address, which pays the network fee.

Your words never leave your device.

## Network

Robinhood Chain testnet. Vault: `0x4136881594De8661b0d4F005AdAFbce67F2FD018`. Every value can be changed on the page under Network settings.

Questions: hello@furtive.app
