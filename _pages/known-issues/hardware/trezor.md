---
title: Trezor
---

{% include hw_experts.md %}

#### No BIP174 Support
TODO: add content

#### Weak Airgap Support
TODO: add content

#### No Keyboard
With only 2 buttons, it's hard to enter a seed phrase (or strong password).
To mitigate this, the Trezor will plug into your computer and use clever tricks to "securely" enter text on your computer.
This is not perfect from a security/UX perspective.

#### No Physical Security
If a clever attacker with ~$100 USD of equipment gains *physical* access to your Trezor (model T or Trezor One) they can extract your seed.
You can read more about this [here](https://donjon.ledger.com/Unfixable-Key-Extraction-Attack-on-Trezor/) and [here](https://blog.kraken.com/post/3662/kraken-identifies-critical-flaw-in-trezor-hardware-wallets/) (Trezor's response [here](https://blog.trezor.io/our-response-to-ledgers-mitbitcoinexpo-findings-194f1b0a97d4)).

These attacks can be mitigated with a strong passphrase, and cannot be exploited remotely (must have physical access to your Trezor).

#### Written in Python
This is not inherently a problem (python is a good general-purpose programming language!), but several hardware wallets with varying level of multisig support are also written in python, such as; Trezor, Coldcard, and Passport.
These hardware wallets share *a lot* of upstream code, and it's possible that if a vulnerability were discovered in one it would be present in the others.

{% include encouragement.md %}
